<template>

    <!-- Card element  -->
    <div class="card col-3">
        <img class="img-fluid" :src="content.image" alt="Recent work">
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
    

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        
    }

}

</style>