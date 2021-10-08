<template>

    <!-- Section containing recent works  -->
    <section class="container-flex">
        <div class="row d-flex justify-content-center text-center">
            <div class="col-6">
                <h2>Explore Recent Work</h2>
                <div class="line"></div>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ea voluptate magni harum quod aperiam nesciunt suscipit placeat iure numquam quaerat ratione, aspernatur enim voluptatum consectetur hic molestias quo ducimus.</p>
            </div>
        </div>

            <div class="row d-flex justify-content-center">
                <RecentWorkCard v-for="(element,index) in cardsContent" :key="index" :content="element" />
            </div>
        
            <div class="row d-flex justify-content-center pt-5 pb-5">
                <div class="left col-2">
                    <div class="line-left"></div>
                </div>

                <div class="col-2 text-center">
                    <span>View all projects</span>
                </div>

                <div class="right col-2">
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

    .left,
    .right {
        
        .line-left,
        .line-right {
            height: 20px;
            width: 100%;
        }

        .line-right {
            border-bottom: 2px solid rgba($silver,.2);
        }

        .line-left {
            border-top: 2px solid rgba($silver,.2);
        }
    }

    span {
        color: $doveGrey;
    }
}

</style>