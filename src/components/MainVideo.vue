<template>
    <div>
        <img class="video-illustration" src="../styles/img/h2-img-2.jpg" alt="video illustration">
        <button><i class="fa-solid fa-caret-right my-icon" style="color:#80ABAE;"></i></button>
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
}

.video-illustration {
    width: 100%;
    height: 100%;
    object-fit: contain;

}

button {
    position: absolute;
    top: 50%;
    right: 50%;
    border: none;
    border-radius: 50%;
    background-color: white;
   
}

.my-icon {
    font-size:  4rem;
    padding: 1.2rem;
}
</style>