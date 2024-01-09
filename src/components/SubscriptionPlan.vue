<template>
    <section class="container-subscriptionPlan">
        <article>
            <h3><strong>Basic</strong></h3>
            <h3 class="price-fs">99<span class="my-dollar-fs">$</span></h3>
        </article>
        <article>
            <h3><strong>Standard</strong></h3>
            <h3 class="price-fs">119<span class="my-dollar-fs">$</span></h3>
        </article>
        <article>
            <h3><strong>Basic</strong></h3>
            <h3 class="price-fs">139<span class="my-dollar-fs">$</span></h3>
        </article>
    </section>
</template>
<script>
export default {
    name:'subscriptionPlan',
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables';
.container-subscriptionPlan{
    width: 60%;
    height: 35rem;
    border: 1px solid red;
    display: flex;
    justify-content: space-between;
    flex-wrap: nowrap;

    h3{
        font-size: variables.$sm-text;
        margin-bottom: 1rem;
    }

    article{
        width: calc((100% / 3) - 2.1rem);
        height: 100%;
        border: 1px solid black;
        border-radius: 2rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 5rem 3rem;
    }

    .price-fs{
        font-size: 2.5rem;
    }

    .my-dollar-fs{
        font-size: 1rem;
        vertical-align: top;
    }
    
}
    
</style>