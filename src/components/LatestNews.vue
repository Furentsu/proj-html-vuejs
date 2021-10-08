<template>

    <!-- Section displaying the latest news  -->
    <section class="container-flex">
        <div class="row d-flex justify-content-center text-center">
            <div class="col-6">
                <h2>Latest News</h2>
                <div class="line"></div>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ea voluptate magni harum quod aperiam nesciunt suscipit placeat iure numquam quaerat ratione, aspernatur enim voluptatum consectetur hic molestias quo ducimus.</p>
            </div>
        </div>

        <div class="row d-flex justify-content-center">
            <LatestNewsCard v-for="(element,index) in cardsContent" :key="index" :content="element" />
        </div>
        

        <div class="row d-flex justify-content-center">
                <div class="col-2">
                    <div class="line-left"></div>
                </div>

                <div class="col-2 text-center p-5">
                    <span>View all projects</span>
                </div>

                <div class="col-2">
                    <div class="line-right"></div>
                </div>
            </div>
    </section>
</template>

<script>
import LatestNewsCard from './LatestNewsCard.vue'

export default {
    name:'LatestNews',
    components: {
        LatestNewsCard,
    },
    data() {
        return {
            cardsContent: [
                {   
                    image: require('../assets/images/blog-post-134132600.jpg'),
                    title: 'Redeveloping Florida\'s Remote Southern Coast',
                    date: 'December 7th, 2015',
                    paragraph: 'lorem'
                },
                {   
                    image: require('../assets/images/blog-post-92486644.jpg'),
                    title: 'How We Manage Large Construction Projects',
                    date: 'December 7th, 2015',
                    paragraph: 'lorem'
                },
                {   
                    image: require('../assets/images/blog-post-332773904.jpg'),
                    title: 'Future proofing a modern home',
                    date: 'December 6th, 2015',
                    paragraph: 'lorem'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
    background-color: rgba($silver,.2);

    h2 {
        padding: 50px 0 20px 0;
        color: $tuatara;
    }

    p {
        color: $doveGrey;
        padding: 20px 0 20px 0;

    }

}

</style>