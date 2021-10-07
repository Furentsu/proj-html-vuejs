<template>

    <!-- Card element  -->
    <div class="card col-2">
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
    border: none;
    
}

</style>