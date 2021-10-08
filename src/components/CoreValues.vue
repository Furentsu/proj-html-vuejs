<template>

    <!-- Section containing the company's core values  -->
    <section class="container-flex">
        <div class="row d-flex justify-content-center text-center">
            <div class="p-5 col-6">
                <h2>Our Core Values</h2>
                <div class="line"></div>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ea voluptate magni harum quod aperiam nesciunt suscipit placeat iure numquam quaerat ratione, aspernatur enim voluptatum consectetur hic molestias quo ducimus.</p>
            </div>
        </div>

        <div class="row d-flex justify-content-center">
            <ValuesCard v-for="(element,index) in cardsContent" :key="index" :content="element" />
        </div>
        
    </section>
</template>

<script>
import ValuesCard from './ValuesCard.vue'

export default {
    name:'ConstructionProjectsBottom',
    components: {
        ValuesCard,
    },
    data() {
        return {
            cardsContent: [
                {   
                    icon: 'fas fa-home',
                    title: 'Great Services',
                    paragraph: 'lorem',
                    bg: 'bali-hai'
                },
                {   
                    icon: 'fas fa-cog',
                    title: 'Highest Standards',
                    paragraph: 'lorem',
                    bg: 'ship-cove'
                },
                {   
                    icon: 'fas fa-users',
                    title: 'Professional Team',
                    paragraph: 'lorem',
                    bg: 'orange'
                },
                {   
                    icon: 'fas fa-lightbulb',
                    title: 'Creative Solutions',
                    paragraph: 'lorem',
                    bg: 'olive'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
    height: 600px;
    background-color: rgba($silver,.2);

    h2 {
        padding: 50px 0 20px 0;
        color: $tuatara;
    }

    p {
        color: $doveGrey;
    }
}

</style>