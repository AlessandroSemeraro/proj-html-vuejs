<template>
    <div>
        <a class="container container-red" href="#"><img src="../styles/svg/svg-2.svg" alt=""> </a>
        <a class="container container-white" href="#"><img src="../styles/svg/svg-4.svg" alt=""> </a>
    </div>
</template>
<script>
export default {
    name: 'icons',
}
</script>
<style lang="scss" scoped>
div {
    display: flex;
    flex-direction: column;
    position: absolute;
    right: 0;
    top: 55%;

}

img{
    width: 0.9rem;
}

.container{
    width: 1.5rem;
    height: 1.5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 0.75rem;
    box-shadow: 0.3px 0.3px 0.3px #888888
}

.container-red{
    background-color: red;
}

.container-white{
    background-color: white;
}
</style>