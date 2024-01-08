<template>
    <section class="container">
        <div class="left-wrapper-MainPresentation">
            <h2>We are Bryson, New <br>
                York-based art & design
                studio</h2>
        </div>
        <div class="right-wrapper-MainPresentation">
            <p>Here at Bryson it only takes a smidgen of imagination and we've already prepared ourselves for future.
                Take a peek and see if you recognize the trademark ingredients of our work.
            </p>
        </div>
    </section>
</template>
<script>
export default {
    name: 'MainPresentation',
    data() {
        return {
        }
    },
}
</script>
<style lang="scss" scoped>
h2 {
    font-size: 2.5rem;
}

p {
    font-size: 0.95rem;
    color: #A6A6A6;
}
.container {
    width: 65%;
    display: flex;
    justify-content: center;
    align-items: center;
    border: 1px solid purple;
    height: 15rem;

    .left-wrapper-MainPresentation {
        width: 50%;
    }

    .right-wrapper-MainPresentation {
        width: 50%;
    }
}
</style>