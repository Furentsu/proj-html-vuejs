<template>

    <!-- Section containing the offered construction services  -->
    <section class="container-flex">
        <div class="row d-flex justify-content-center text-center">
            <div class="p-5 col-6">
                <h2 class="fw-light">Specialists In Modern Construction</h2>
                <div class="line"></div>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ea voluptate magni harum quod aperiam nesciunt suscipit placeat iure numquam quaerat ratione, aspernatur enim voluptatum consectetur hic molestias quo ducimus.</p>
            </div>
        </div>

        <div class="row d-flex justify-content-center pb-5">
            <ConstructionProjectsCard class="mb-5" v-for="(element,index) in cardsContent" :key="index" :content="element" />
        </div>
        
    </section>
</template>

<script>
import ConstructionProjectsCard from './ConstructionProjectsCard.vue'

export default {
    name:'ConstructionProjectsBottom',
    components: {
        ConstructionProjectsCard,
    },
    data() {
        return {
            cardsContent: [
                {   
                    icon: 'fas fa-building',
                    title: 'Buildings',
                    paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {   
                    icon: 'fas fa-sync-alt',
                    title: 'Renovate',
                    paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {   
                    icon: 'fas fa-home',
                    title: 'Construct',
                    paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {   
                    icon: 'fas fa-truck',
                    title: 'Exclusive',
                    paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
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