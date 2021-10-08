<template>

    <!-- Section containing trusted partners  -->
    <section class="container-flex">
        <div class="row d-flex justify-content-center text-center">
            <div class="col-6">
                <h2>Trusted Partners</h2>
                <div class="line"></div>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ea voluptate magni harum quod aperiam nesciunt suscipit placeat iure numquam quaerat ratione, aspernatur enim voluptatum consectetur hic molestias quo ducimus.</p>
            </div>
        </div>

        <div class="row row-cols-5 d-flex justify-content-center">
            <TrustedPartnersCard v-for="(element,index) in cardsContent" :key="index" :content="element" />
        </div>
        
    </section>
</template>

<script>
import TrustedPartnersCard from './TrustedPartnersCard.vue'


export default {
    name:'ConstructionProjectsBottom',
    components: {
        TrustedPartnersCard,
    },
    data() {
        return {
            cardsContent: [
                {   
                    logo: require('../assets/images/home-logo11-219096700-320x202.png')
                },
                {   
                    logo: require('../assets/images/home-logo10-219096700-320x202.png')
                },
                {   
                    logo: require('../assets/images/home-logo2-219096700-320x202.png')
                },
                {   
                    logo: require('../assets/images/home-logo1-219096700-320x202.png')
                },
                {   
                    logo: require('../assets/images/home-logo9-219096700-320x202.png')
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
    height: 500px;

    h2 {
        padding-top: 50px;
        color: $tuatara;
    }

    .line {
        height: 2px;
        width: 30%;
        margin: 20px auto;
        background-color: $vibrantBrightSun;
    }

    p {
        color: $doveGrey;
    }
}

</style>