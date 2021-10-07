<template>

    <!-- Section containing the offered construction services  -->
    <section class="container-flex">
        <div class="row">
            <div class="col-6">
                <h2>Our Core Values</h2>
                <div class="line"></div>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ea voluptate magni harum quod aperiam nesciunt suscipit placeat iure numquam quaerat ratione, aspernatur enim voluptatum consectetur hic molestias quo ducimus.</p>
            </div>
        </div>

        <div class="row">
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
                    icon: 'fas fa-building',
                    title: 'Great Services',
                    paragraph: 'lorem'
                },
                {   
                    icon: 'fas fa-sync-alt',
                    title: 'Highest Standards',
                    paragraph: 'lorem'
                },
                {   
                    icon: 'fas fa-home',
                    title: 'Professional Team',
                    paragraph: 'lorem'
                },
                {   
                    icon: 'fas fa-truck',
                    title: 'Creative Solutions',
                    paragraph: 'lorem'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
    border: 1px solid black;

    height: 550px;
}

</style>