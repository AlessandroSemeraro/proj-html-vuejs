<template>
    <header>
        <nav>
            <div>
                <img src="C:\Users\alese\OneDrive\Desktop\Boolean\js\proj-html-vuejs\src\styles\img\logo-img-01.png" alt="">
            </div>
            <div>a</div>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data(){
        return {
        }
    },
}


</script>

<style lang="scss" scoped>
header{
    height: 6rem;
    border:1px solid black;
    
    nav{
        height: 100%;
        padding: 0 2rem;
        display: flex;
        align-items: center;
        justify-content: space-between;

        img{
            width: 4rem;
        }
    }
}
</style>