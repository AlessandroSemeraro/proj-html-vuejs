<template >
    <section class="footerBottom">
        <a href="#"><img class="logo" src="../styles/img/logo-img-01.png" alt="logo icon"></a>
        <p>Sometimes doing something seemingly demanding turns out to be fun. <br>
            Here's the proof - Bryson, your brand new portfolio.
        </p>
        <div class="footerSocials">
            <SocialsFooter :socialsList="socialsList"/>
        </div>
    </section>
</template>
<script>
import SocialsFooter from './SocialsFooter.vue';

export default {
    name: 'contacts',
    data() {
        return {
            socialsList: [
                {
                    iconClass: "fa-instagram",
                    name: "instagram",
                    bgColor: "#69A9AA"                   
                },
                {
                    iconClass: "fa-facebook-f",
                    name: "facebook",
                    bgColor:"#EEc681"
                },
                {
                    iconClass: "fa-twitter",
                    name: "twitter",
                    bgColor:"#f7bca8"
                    
                },
                {
                    iconClass: "fa-pinterest-p",
                    name: "pinteres",
                    bgColor:"#D8D597"
                }
            ]
        };
    },
    components: { SocialsFooter }
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables';

.footerBottom {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 20rem;
    background-color: #E6F3F0;
    background-image: url(../styles/img/h2-footer-img-01.jpg);
    background-size: cover;
}
.logo {
    width: 5rem;
    margin-bottom: 0.75rem;
}

p {
    font-size: variables.$sm-text;
    line-height: variables.$space-lines;
    text-align: center;
    margin-bottom: 1.25rem;
    font-weight: 200;
}

.footerSocials {
    display: flex;
}


</style>