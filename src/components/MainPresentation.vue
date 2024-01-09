<template>
    <section class="container-presentation">
        <div class="left-wrapper-MainPresentation">
            <h2>We are Bryson, New
                York-based art & design
                studio</h2>
        </div>
        <div class="right-wrapper-MainPresentation">
            <p>Here at Bryson it only takes a smidgen of imagination and we've already prepared ourselves for future
                challenges.
                Take a peek and see if you recognize the trademark ingredients of our work.
            </p>
        </div>
    </section>

    <section class="container-cards">
        <MainCards v-for="card in cardsList" :imageSrc="card.src" />
    </section>
</template>
<script>
import MainCards from './MainCards.vue';

export default {
    name: 'MainPresentation',
    data() {
        return {
            cardsList: [
                {
                    src: "src/styles/img/port-img-07.jpg"
                },
                {
                    src: "src/styles/img/port-img-08.jpg"
                },
                {
                    src: "src/styles/img/port-img-09.jpg"
                },
                {
                    src: "src/styles/img/port-img-10.jpg"
                },
                {
                    src: "src/styles/img/port-img-11.jpg"
                },
                {
                    src: "src/styles/img/port-img-12.jpg"
                },
            ]
        };
    },
    components: { MainCards }
}
</script>
<style lang="scss" scoped>
h2 {
    font-size: 2.85rem;
}

p {
    font-size: 0.85rem;
    color: #A6A6A6;
}


.container-presentation {
    width: 65%;
    padding-top: 5rem;
    padding-bottom: 16rem;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;

    .left-wrapper-MainPresentation {
        width: 50%;
        margin-right: 3.75rem;
    }

    .right-wrapper-MainPresentation {
        width: 50%;
    }
}

.container-cards {
    position: absolute;
    top: 30rem;
    width: 60%;
    display: flex;
    flex-wrap: wrap;
}


</style>
