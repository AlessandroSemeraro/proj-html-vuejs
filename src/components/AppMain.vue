

<template>
    <main>
    <MainPresentation />
    

    </main>
</template>

<script>

import MainPresentation from './MainPresentation.vue';

export default {
name: 'AppMain',

components: {
    MainPresentation
},
}
</script>
<style lang="scss" scoped>
    main{
        height: 100rem;
        background-size: 85%;
        background-image:url(../styles/img/h2-background-img-02.png) ;
        background-repeat: repeat-x;
        display: flex;
        justify-content: center;
    }
</style>