<template>

    <!-- Card element  -->
    <div class="card col-3">
        <div class="icon-container">
            <i :class="content.icon"></i>
        </div>
        <div class="line"></div>
        <h2>{{content.title}}</h2>
        <p>{{content.paragraph}}</p>
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
    
    height: 200px;

    .icon-container {
    border: 1px solid blue;

        width: 50px;
        height: 50px;
    }
}

</style>