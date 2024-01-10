<template>
   <section>
        <FooterUpper/>
   </section> 
   <section>
        <FooterBottom/>
   </section>
</template>

<script>
import FooterBottom from './FooterBottom.vue';
import FooterUpper from './FooterUpper.vue';


export default {
    name: 'AppFooter',
    data() {
        return {};
    },
    components: { FooterUpper, FooterBottom }
}
</script>
<style lang="scss" scoped>
    
</style>