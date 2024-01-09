<template>
    <header>
        <nav>

            <!-- LOGO -->
            <section class="left-nav">
                <img class="logo" src="../styles/img/logo-img-01.png" alt="">
            </section>

            <!-- MENU -->
            <section class="right-nav">
                <div class="align-items">
                    <a v-for="item, index in navElements" :href="item.link" :key="index">
                        {{ item.text }}
                    </a>
                </div>
                <div class="align-items">
                    <a class="icon-item" href="#"><img src="../styles/svg/svg-1.svg" alt="bullets"></a>
                </div>
            </section>

        </nav>
    </header>
</template>

    <!--!!!!!!!!!!!!!!!ACTIVE INDEX TORNA!!!!!!!!!!!!!!!!!!!!!-->
<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            currentActive: 1,
        }
    },
    methods: {
        setCurrentActive(index) {
            this.currentActive = index;
        }
    },
    props: {
        navElements: Array,
    },
}


</script>

<style lang="scss" scoped>
header {
    height: 6rem;

    nav {
        height: 100%;
        padding: 0 2.5rem;
        display: flex;
        align-items: center;
        justify-content: space-between;

        .logo {
            width: 4rem;
        }
    }
}
.left-nav {
    display: flex;
    align-items: center;
}
.right-nav {
    display: flex;

    .align-items {
        display: flex;
        align-items: center;

    }
}

a {
    color: black;
    text-decoration: none;
    padding: 0 1rem;
    margin-right: 2rem;
}

.icon-item {
    padding-right: 0;
}

.bottom-line {
    border-bottom: 3px solid brown;
}
</style>