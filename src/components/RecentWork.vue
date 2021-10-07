<template>

    <!-- Section containing recent works  -->
    <section class="container-flex">
        <div class="row">
            <div class="col-6">
                <h2>Explore Recent Work</h2>
                <div class="line"></div>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ea voluptate magni harum quod aperiam nesciunt suscipit placeat iure numquam quaerat ratione, aspernatur enim voluptatum consectetur hic molestias quo ducimus.</p>
            </div>
        </div>

            <div class="row">
                <RecentWorkCard v-for="(element,index) in cardsContent" :key="index" :content="element" />
            </div>
        
            <div class="row">
                <div class="col-3">
                    <div class="line-left"></div>
                </div>

                <div class="col-3">
                    <h3>View all projects</h3>
                </div>

                <div class="col-3">
                    <div class="line-right"></div>
                </div>
            </div>

    </section>
</template>

<script>
import RecentWorkCard from './RecentWorkCard.vue'

export default {
    name:'ConstructionProjectsBottom',
    components: {
        RecentWorkCard,
    },
    data() {
        return {
            cardsContent: [
                {   
                    image: require('../assets/images/project2-featured-15013609.jpg'),
                },
                {   
                    image: require('../assets/images/project1-featured-294276386.jpg'),
                },
                {   
                    image: require('../assets/images/project3-featured-189023420.jpg'),
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
    border: 2px solid black;

    height: 550px;
}

</style>