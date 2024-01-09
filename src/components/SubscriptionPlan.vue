<template>
    <section class="container-subscriptionPlan">
        <article></article>
        <article></article>
        <article></article>
    </section>
</template>
<script>
export default {
    name:'subscriptionPlan',
}
</script>
<style lang="scss" scoped>

.container-subscriptionPlan{
    width: 60%;
    height: 35rem;
    border: 1px solid red;
    display: flex;
    justify-content: space-between;
    flex-wrap: nowrap;

    article{
        width: calc((100% / 3) - 2.1rem);
        height: 100%;
        border: 1px solid black;
        border-radius: 2rem;
        
    }
    
}
    
</style>