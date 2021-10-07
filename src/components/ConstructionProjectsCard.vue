<template>

    <!-- Card element  -->
    <div class="card col-2">
        <div class="icon-container">
            <i :class="content.icon"></i>
        </div>
        <h2 class="fw-light">{{content.title}}</h2>
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
    border: 1px solid transparent;
    border-radius: 5px;
    margin: 0 15px;
    background-color: rgba($silver, .2);
    height: 200px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .icon-container {
        border: 1px solid $stormDust;
        border-radius: 2em;

        width: 50px;
        height: 50px;
        display: flex;
        align-items: center;
        justify-content: center;

        i {
            font-size: 1.3rem;
            color: $stormDust;
        }
    }
}

</style>