<template>

    <!-- Card element  -->
    <div class="card col-3">
        <div class="img-container">
            <img :src="content.image" alt="Blog post image">
        </div>
        <div class="card-content">
            <h2>{{content.title}}</h2>
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
    border: 1px solid red;
    
    .img-container {
        width: 100%;

        img {
            width: 100%;
        }
    }

}

</style>