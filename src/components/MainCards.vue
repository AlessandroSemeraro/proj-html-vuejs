<template >
    <article>
        <img :src="imageSrc" alt="CardsPresentation">
    </article>
</template>

<script>

export default {
    name: 'MainCards',
    props: {
        imageSrc : {
            type :[
                String
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    article{
        width: calc((100% / 2));
        display: flex;
        flex-wrap: nowrap;
        height: 33rem;

        img{
            width: 100%;
        }
    }
</style>