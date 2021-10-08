<template>

    <!-- Card element  -->
    <div class="card col-2 pt-3 text-center">
        <div class="icon-container">
            <i :class="content.icon"></i>
        </div>
        <h2 class="fw-light pt-2">{{content.title}}</h2>
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
    width: 300px;
    border: 1px solid transparent;
    border-radius: 5px;
    margin: 0 15px;
    background-color: rgba($silver, .2);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;

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