<script>

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {
      navElements: [
        {
          text: 'Home',
          link: '#',
        },
        {
          text: 'Pages',
          link: '#',
        },
        {
          text: 'Portfolio',
          link: '#',
        },
        {
          text: 'Blog',
          link: '#',
        },
        {
          text: 'Shop',
          link: '#',
        },
        {
          text: 'Elements',
          link: '#',
        },
      ],
    }
  },
  components:{
    AppHeader,
    AppMain,
    AppFooter
  }
  
}
</script>

<template>
  <AppHeader :navElements="navElements"/>
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss';


</style>
