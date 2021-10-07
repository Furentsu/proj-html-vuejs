<template>

    <!-- Card element  -->
    <div class="card col-3">
        <div class="img-container">
            <img :src="content.image" alt="Blog post image">
        </div>
        <div class="card-content">
            <h2 class="fw-light mt-4">{{content.title}}</h2>
            <span>{{content.date}}</span>
            <div class="line"></div>
            <p>{{content.paragraph}}</p>
        </div>
    </div>
</template>

<script>

export default {
    name:'ConstructionProjectsCard',
    props: ['content']
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.card {

    border: none;
    padding: 0 0;
    margin: 0 15px;
    
    .img-container {
        width: 100%;

        img {
            width: 100%;
        }
    }

    .card-content {
        padding: 0 10px;

        h2 {
            font-size: 1.4rem;
        }

        span {
            font-size: .9rem;
        }
    }

}

</style>