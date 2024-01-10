<template >
    <section class="socials">
        <div class="container-icon bg-green">
            <a href="#"><i class="my-icon fa-brands fa-instagram" style="color: #000000;"></i> </a>
        </div>
        <div class="container-icon bg-orange">
            <a href="#"><i class="my-icon fa-brands fa-facebook-f" style="color: #000000;"></i> </a>
        </div>
        <div class="container-icon bg-pink">
            <a href="#"><i class="my-icon fa-brands fa-twitter" style="color: #000000;"></i> </a>
        </div>
        <div class="container-icon bg-yellow">
            <a href="#"><i class="my-icon fa-brands fa-pinterest-p" style="color: #000000;"></i> </a>
        </div>
    </section>
</template>
<script>
export default {
    name: 'socials',
}
</script>
<style lang="scss" scoped>
.socials {
    display: flex;
    flex-direction: column;
    position: absolute;
    right: 2%;
    top: 20%;

    .container-icon {
        margin-bottom: 1rem;
        height: 2rem;
        width: 2rem;
        border-radius: 50%;
        color: transparent;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .bg-green:hover {
        background-color: #69A9AA;

        .my-icon {
            color: white !important;
        }
    }

    .bg-orange:hover {
        background-color: #EEc681;

        .my-icon {
            color: white !important;
        }
    }

    .bg-pink:hover {
        background-color: #f7bca8;

        .my-icon {
            color: white !important;
        }
    }

    .bg-yellow:hover {
        background-color: #D8D597;

        .my-icon {
            color: white !important;
        }
    }
}
</style>