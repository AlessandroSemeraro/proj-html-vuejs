

<template>
    <main>
        <section class="mainPresentation-upper">
            <MainPresentation />
        </section>
        <section class="mainPresentation-bottom">
            
        </section>

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
.mainPresentation-upper {
    background-size: 85%;
    background-image: url(../styles/img/h2-background-img-02.png);
    background-repeat: repeat-x;
    display: flex;
    flex-direction: column;
    align-items: center;
    border: 4px solid red;
}

.mainPresentation-bottom {
    height: 100rem;
    background-size: 85%;
    background-image: url(../styles/img/h3-background-img-03.png);
    background-repeat: repeat-x;
}
</style>