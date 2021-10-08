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
        
        
        <div class="row d-flex justify-content-center pt-5 pb-5">
                <div class="left col-3">
                    <div class="line-left"></div>
                </div>

                <div class="col-3 text-center">
                    <span>View all projects</span>
                </div>

                <div class="right col-3">
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
                    paragraph: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Porro ipsam dolorem ratione reiciendis blanditiis sequi repudiandae, officia adipisci pariatur. Mollitia necessitatibus explicabo doloremque distinctio et dicta nobis vel repudiandae fugit.'
                },
                {   
                    image: require('../assets/images/blog-post-92486644.jpg'),
                    title: 'How We Manage Large Construction Projects',
                    date: 'December 7th, 2015',
                    paragraph: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Porro ipsam dolorem ratione reiciendis blanditiis sequi repudiandae, officia adipisci pariatur. Mollitia necessitatibus explicabo doloremque distinctio et dicta nobis vel repudiandae fugit.'
                },
                {   
                    image: require('../assets/images/blog-post-332773904.jpg'),
                    title: 'Future proofing a modern home',
                    date: 'December 6th, 2015',
                    paragraph: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Porro ipsam dolorem ratione reiciendis blanditiis sequi repudiandae, officia adipisci pariatur. Mollitia necessitatibus explicabo doloremque distinctio et dicta nobis vel repudiandae fugit.'
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
        padding: 20px 0 20px 0;

    }

    .left,
    .right {
        margin: 0 20px;
        padding: 0 10px;
        
        .line-left,
        .line-right {
            height: 20px;
            width: 100%;
        }

        .line-right {
            border-bottom: 2px solid $primaryWhite;
        }

        .line-left {
            border-top: 2px solid $primaryWhite;
        }
    }

    span {
        color: $doveGrey;
    }


}

</style>