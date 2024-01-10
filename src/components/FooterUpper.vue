<template >
    <section class="footerUpper">
        <div class="container-upper">
            <div class="form-description-container">
                <h3>Get in touch <br>
                    and say hello</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Culpa repudiandae reprehenderit assumenda. Illum odio debitis, molestias qui deleniti obcaecati.</p>
            </div>
            <div class="form-container">
                <form>
                    <section>
                        <textarea v-model="comments" type="text" class="my-form form-large" placeholder="Comment"></textarea>
                        <input v-model="name"  type="text" placeholder="Name" class="my-form form-small form-mr">
                        <input v-model="email" type="text" placeholder="Email" class="my-form form-small">
                    </section>
                    <div>
                        <a @click="submitted" href="#" class="myButton"><strong>Submit <i class="fa fa-solid fa-caret-right arrow"></i></strong></a>
                    </div>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
export default {

    name: 'form',

    data(){
        return{
        
        comments:'',
        name:'',
        email:''
        
    }
},

methods :{
    submitted (){
        alert('Grazie ' + this.name + ' , il form è stato inviato correttamente!')
    }
}
    

}

</script>
<style lang="scss" scoped>
@use '../styles/partials/variables';

.footerUpper {
    display: flex;
    justify-content: center;
    align-items: center;
}

.container-upper {
    width: 60%;
    display: flex;
    padding: 6rem 0;
}

.form-description-container {
    width: 35%;
}


h3 {
    font-size: variables.$md-text;
    margin-bottom: 1rem;
}

p {
    font-size: variables.$sm-text;
    line-height: variables.$space-lines;
    font-weight: 200;
}


.form-container {
    width: 65%;
    display: flex;
    justify-content: center;
    
}

.my-form{
    height: 1.6rem;
    border-top: none;
    border-right: none;
    border-left: none;
    border-bottom: 1.5px solid black;
}

.form-large{
    width: 28rem;
    display: block;
    margin-top: 0.5rem;
    margin-bottom: 2rem;
}

textarea {
  resize: vertical;
  outline: none;
}

input{
    outline:none
}

.form-small{
    width: 13rem;
    margin-bottom: 3rem;
}

.form-mr{
    margin-right: 2rem;
}

.myButton {
        width: 9rem;
        background-color: white;
        border-radius: 25px;
        border: 1.5px solid #80ABAE;
        display: inline-block;
        cursor: pointer;
        color: #000000;
        font-family: Arial;
        font-size: 12px;
        padding: 12px 10px;
        text-decoration: none;
        text-align: center;
    }

    i{
        vertical-align: baseline;
    }
    .myButton:hover {
        color: white;
        background-color: #80ABAE;
    }

    .myButton:hover i {
        fill: white;
    }


</style>