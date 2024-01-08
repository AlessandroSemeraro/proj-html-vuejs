
<template>
    <main>
        <section class="mainBgPresentation-upper">
            <MainPresentation />
        </section>
        <section class="mainBgPresentation-lower">
        </section>
        <section class="main-bottom">
            <MainBottom />
        </section>

    </main>
</template>

<script>

import MainPresentation from './MainPresentation.vue';
import MainBottom from './MainBottom.vue';

export default {
    name: 'AppMain',

    components: {
        MainPresentation,
        MainBottom,
    },
}
</script>
<style lang="scss" scoped>
.mainBgPresentation-upper {
    background-size: 85%;
    background-image: url(../styles/img/h2-background-img-02.png);
    background-repeat: repeat-x;
    display: flex;
    flex-direction: column;
    align-items: center;
    border: 4px solid red;
}

.mainBgPresentation-lower {
    height: 92rem;
    background-size: 85%;
    background-image: url(../styles/img/h3-background-img-03.png);
    background-repeat: repeat-x;
}

.main-bottom{
    display: flex;
    justify-content: center;
}

</style>