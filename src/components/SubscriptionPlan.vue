<template>
    <section class="container-subscriptionPlan">
        <article>
            <h3><strong>Basic</strong></h3>
            <h3 class="price-fs">99<span class="my-dollar-fs">$</span></h3>
            <p>5 Design concepts </p>
            <p>Full copyright ownership </p>
            <p>Art direction </p>
            <p>Top level creatives </p>
            <p>No money back </p>
            <a href="#" class="myButton"><strong>Read more <i class="fa fa-solid fa-caret-right arrow"></i></strong></a>
        </article>
        <article>
            <h3><strong>Standard</strong></h3>
            <h3 class="price-fs">119<span class="my-dollar-fs">$</span></h3>
            <p>10 Design concepts </p>
            <p>Full copyright ownership </p>
            <p>Art direction </p>
            <p>Top level creatives </p>
            <p>No money back </p>
            <a href="#" class="myButton myButtonBg"><strong>Read more <i class="fa fa-solid fa-caret-right arrow"></i></strong></a>
        </article>
        <article>
            <h3><strong>Basic</strong></h3>
            <h3 class="price-fs">139<span class="my-dollar-fs">$</span></h3>
            <p>15 Design concepts </p>
            <p>Full copyright ownership </p>
            <p>Art direction </p>
            <p>Top level creatives </p>
            <p>No money back </p>
            <a href="#" class="myButton"><strong>Read more <i class="fa fa-solid fa-caret-right arrow"></i></strong></a>
        </article>
    </section>
    
</template>
<script>

export default {
    name: 'subscriptionPlan',
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables';

.container-subscriptionPlan {
    width: 60%;
    height: 33rem;
    display: flex;
    justify-content: space-between;
    flex-wrap: nowrap;

    h3 {
        font-size: variables.$sm-text;
    }

    p {
        font-size: variables.$sm-text;
        font-weight: 200;
        line-height: variables.$space-lines;
    }

    h3,
    p {
        margin-bottom: 1rem;
    }

    
    article {
        width: calc((100% / 3) - 2.1rem);
        border-radius: 2rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    article:first-child{
            border:1.5px solid #EFCA9E;
        }
    
    article:nth-child(2){
        background-color: #E6F3F0;
            border: none 
    }

    article:last-child{
        border:1.5px solid #EA9B82;
    }

    .price-fs {
        font-size: 2.5rem;
    }

    .my-dollar-fs {
        font-size: 1rem;
        vertical-align: top;
    }
    .myButton {
        margin-top: 2rem;
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

    .myButtonBg{
        background-color: transparent;
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

}
</style>