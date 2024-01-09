<template >
    <div>
        <a href="#"><i class="fa-brands fa-instagram" style="color: #000000;"></i> </a>
        <a href="#"><i class="fa-brands fa-facebook-f" style="color: #000000;"></i> </a>
        <a href="#"><i class="fa-brands fa-twitter" style="color: #000000;"></i> </a>
        <a href="#"><i class="fa-brands fa-pinterest-p" style="color: #000000;"></i> </a>
    </div>
</template>
<script>
export default {
    name: 'socials',
}
</script>
<style lang="scss" scoped>
    div{
        display: flex;
        flex-direction: column;
        position: absolute;
        right: 2%;
        top: 5%;
        
        div i {
            margin-top: 1.5rem;
        }
    }
</style>