<template>
    <div>
        <button><i class="fa-solid fa-caret-right my-icon my-icon-orange" style="color:#80ABAE;"></i></button>
    </div>
</template>
<script>
export default {
    name: 'mainVideo',
}
</script>
<style lang="scss" scoped>
div {
    width: 100%;
    height: 100%;
    position: relative;
    background-image: url(../styles/img/h2-img-2.jpg);
    background-size:75%;
    background-position: 15rem 10rem;
}


.video-illustration {
    width: 100%;
    height: 100%;
    object-fit: cover;

}

button {
    position: absolute;
    top: 45%;
    right: 50%;
    border: none;
    border-radius: 50%;
    background-color: white;
    cursor: pointer;
}



.my-icon {
    font-size:  4rem;
    padding: 1.2rem;
}

.my-icon-orange:hover{
    color: #EAc3AD !important;
}
</style>