<template >
    <section class="container-mainBottom">
        <div class="container-left-mainBottom">
            <h2>What we do?</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Culpa repudiandae reprehenderit assumenda. Illum odio debitis, molestias qui deleniti obcaecati id aliquam 
                optio a corrupti perferendis minus voluptate veritatis doloribus nemo!</p>
        </div>
        <div class="container-right-mainBottom"></div>
    </section>
</template>
<script>
export default {
    name: 'MainBottom',
}
</script>
<style lang="scss" scoped>
    .container-mainBottom{
        width:60%;
        height: 30rem;
        border: 1px solid magenta;
        display: flex;
    }
    .container-left-mainBottom{
        width: 40%;
        border: 1px solid black;
        display: flex;
        align-items: center;
        flex-direction: column;
    }

    .container-right-mainBottom{
        width: 60%;
        border: 1px solid black;
        display: flex;
    }
</style>