
<template>
    <main>
        <section class="mainBgPresentation-upper">
            <MainPresentation />
        </section>
        <section class="mainBgPresentation-lower">
        </section>
        <section class="main-bottom-pres">
            <MainBottomPresentation />
            <Socials/>
        </section>
        <section class="main-video">
            <MainVideo/>
        </section>
        <section class="mainBg-subscription">
            <SubscriptionPlan/>
            <SvgIcons/>
        </section>
    </main>
</template>

<script>

import MainPresentation from './MainPresentation.vue';
import MainBottomPresentation from './MainBottomPresentation.vue';
import Socials from './Socials.vue';
import MainVideo from './MainVideo.vue';
import SubscriptionPlan from './SubscriptionPlan.vue';
import SvgIcons from './SvgIcons.vue';

export default {
    name: 'AppMain',

    components: {
    MainPresentation,
    MainBottomPresentation,
    Socials,
    MainVideo,
    SubscriptionPlan,
    SvgIcons,
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
}

.mainBgPresentation-lower {
    height: 92rem;
    background-size: 85%;
    background-image: url(../styles/img/h3-background-img-03.png);
    background-repeat: repeat-x;
}

.main-bottom-pres{
    display: flex;
    justify-content: center;
    position: relative;
}

.main-video{
    height: 30rem;
}

.mainBg-subscription{
    display: flex;
    justify-content: center;
    height: 50rem;
    background-image: url(../styles/img/h2-background-img-03.png);
    background-position: 0 -3rem;
    padding-top: 10rem;
    position: relative;
}

</style>