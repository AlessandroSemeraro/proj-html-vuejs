<template>
    <div v-for="social in socialsList" class="container-icon">
        <a href="#">
            <div class="bg-icon-circle" :style="{backgroundColor: social.bgColor}"><i class="fa-brands" :class="social.iconClass"  style="color: #ffffff;"></i>
            </div>
        </a>
    </div>
</template>
<script>
export default {
    props: {
        socialsList : {
            type :[
                Object
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
.container-icon {
    margin-right: 1rem;
}

a {
    text-decoration: none;
}

.bg-icon-circle {
    height: 2rem;
    width: 2rem;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
}

</style>