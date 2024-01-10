<template>
    <header>
        <nav>

            <!-- LOGO -->
            <section class="left-nav">
                <a href="#"><img class="logo" src="../styles/img/logo-img-01.png" alt="logo icon"></a>
            </section>

            <!-- MENU -->
            <section class="right-nav">
                <div class="align-items">
                        <a  v-for="item, index in navElements" :class="{ active:index===currentActive }" @click="setCurrentActive(index)" :href="item.link" :key="index">
                           {{ item.text }} 
                        </a>                   
                </div>
                <div class="align-items">
                    <a class="icon-item" href="#"><img src="../styles/svg/svg-1.svg" alt="bullets"></a>
                </div>
            </section>

        </nav>

            <!--ARROW LATERAL-->
        <div>
            <a href="#top"><i class="myArrow first-arrow fa-solid fa-caret-up" style="color: #f6c0ab;"><span><i class="myChevron fa-solid fa-chevron-up" style="color: #ffffff;"></i></span></i></a>
            <a href="#top"><i class="myArrow second-arrow fa-solid fa-caret-up" style="color: #f6c0ab;"><span><i class="myChevron fa-solid fa-chevron-up" style="color: #ffffff;"></i></span></i></a>
            <a href="#top"><i class="myArrow third-arrow fa-solid fa-caret-up" style="color: #f6c0ab;"><span><i class="myChevron fa-solid fa-chevron-up" style="color: #ffffff;"></i></span></i></a>
            <a href="#top"><i class="myArrow fourth-arrow fa-solid fa-caret-up" style="color: #f6c0ab;"><span><i class="myChevron fa-solid fa-chevron-up" style="color: #ffffff;"></i></span></i></a>
            <a href="#top"><i class="myArrow fifth-arrow fa-solid fa-caret-up" style="color: #f6c0ab;"><span><i class="myChevron fa-solid fa-chevron-up" style="color: #ffffff;"></i></span></i></a>
            <a href="#top"><i class="myArrow sixth-arrow fa-solid fa-caret-up" style="color: #f6c0ab;"><span><i class="myChevron fa-solid fa-chevron-up" style="color: #ffffff;"></i></span></i></a>
            <a href="#top"><i class="myArrow seventh-arrow fa-solid fa-caret-up" style="color: #f6c0ab;"><span><i class="myChevron fa-solid fa-chevron-up" style="color: #ffffff;"></i></span></i></a>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            currentActive: 0,
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
    position: relative;

    nav {
        height: 100%;
        padding: 0 2.5rem;
        display: flex;
        align-items: center;
        justify-content: space-between;

        .logo {
            width: 4rem;
            cursor: pointer;
        }
    }

    .myArrow{
        font-size: 5rem;
        position: relative;
        .myChevron{
            font-size:8px;
            position:absolute;
            top: 33px;
            left: 22px;
        }
    }

    .first-arrow{
        position: absolute;
        right: 2rem;
        top: 70rem;
    }

    .second-arrow{
        position: absolute;
        right: 2rem;
        top:108rem;
    }

    .third-arrow{
        position: absolute;
        right: 2rem;
        top:145rem;
        z-index: 1;
    }

    .fourth-arrow{
        position: absolute;
        right: 2rem;
        top:172rem;
        z-index: 1;
    }
    .fifth-arrow{
        position: absolute;
        right: 2rem;
        top:207rem;
        z-index: 1;
    }
    .sixth-arrow{
        position: absolute;
        right: 2rem;
        top:241rem;
    }
    .seventh-arrow{
        position: absolute;
        right: 2rem;
        top:276rem;
    }
}

.active{

    text-decoration: underline;
    text-decoration-color: #ea9b82;
    text-decoration-style: solid;
    text-decoration-thickness: 1px;
    text-underline-offset: 8px;
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