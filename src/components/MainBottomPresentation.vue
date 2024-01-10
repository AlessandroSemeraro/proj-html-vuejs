<template >
    <section class="container-mainBottom">
        <div class="container-left-mainBottom">
            <h3>What we do?</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Culpa repudiandae reprehenderit assumenda.
                Dolor pretium quis sem.  </p>
            <a href="#" class="myButton"><strong>Read more <i class="fa fa-solid fa-caret-right arrow"></i></strong></a>
        </div>
        <div class="container-right-mainBottom">
            <article>
                <div>
                    <img src="../styles/img/h2-icon-01.png" alt="pink leaf">
                    <p><strong> Beautifull <br> illustrations </strong></p>
                </div>
            </article>
            <article>
                <div>
                    <img src="../styles/img/h2-icon-02.png" alt="cartoon clouds">
                    <p><strong> Brand <br> strategies </strong></p>
                </div>
            </article>
            <article>
                <div>
                    <img src="../styles/img/h2-icon-03.png" alt="blue umbrella">
                    <p><strong> Qualified <br> support </strong></p>
                </div>
            </article>
            <article>
                <div>
                    <img src="../styles/img/h2-icon-04.png" alt="orange books">
                    <p><strong> Books & <br> magazines </strong></p>
                </div>
            </article>
        </div>
    </section>
</template>
<script>
export default {
    name: 'MainBottom',
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables';

.container-mainBottom {
    width: 60%;
    padding: 6rem 0;
    display: flex;
}

.container-left-mainBottom {
    width:40%;
    margin-top: 1.5rem;
    margin-right: 3rem;
    display: flex;
    flex-direction: column;

    h3{
        font-size: variables.$md-text;
        margin-bottom: 1rem;
    }

    p {
        font-size: variables.$sm-text;
        font-weight: 200;
        line-height: variables.$space-lines;
        margin-bottom: 1.75rem;
    }

    .myButton {
        width: 10rem;
        background-color: white;
        border-radius: 25px;
        border: 1.5px solid #80ABAE;
        display: inline-block;
        cursor: pointer;
        color: #000000;
        font-family: Arial;
        font-size: 12px;
        padding: 12px 20px;
        text-decoration: none;
        text-align: center;

    }

    i{
        vertical-align:baseline;
    }
    .myButton:hover {
        color: white;
        background-color: #80ABAE;
    }

    .myButton:hover i {
        fill: white;
    }

    .arrow{
        margin-left: 0.1rem;
    }

}

.container-right-mainBottom {
    width: 60%;
    display: flex;
    flex-wrap: wrap;

    img{
        width: 4rem;
    }

    article{
        width: calc(100% / 2);
        display: flex;
        justify-content: center;
        align-items: center;
        padding:2rem 5rem 0 5rem;
        cursor: pointer;
        

        div{
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 0.9rem 1.5rem 0.9rem 1.5rem;
        border: 1.5px solid transparent;
        margin-bottom: 0.25rem;
        }

        div:hover{
        border: 1.5px solid #E5A85A;
        border-radius: 20px;
        
        }
        img{
            margin-right: 1.5rem;
        }
    }
}
</style>