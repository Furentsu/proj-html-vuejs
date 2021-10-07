<template>

    <!-- Card element  -->
    <div class="card col-2">
        <div class="icon-container">
            <i :class="content.icon"></i>
        </div>
        <h2>{{content.number}}</h2>
        <p>{{content.title}}</p>
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
    background-color: transparent;
    height: 200px;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .icon-container {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 80px;
        height: 80px;

        i {
            font-size: 3rem;
            color: $vibrantBrightSun;
        }
        
    }

    h2 {
        color: $vibrantBrightSun;
    }

    p {
        font-size: 1.1rem;
        color: $primaryWhite;
    }
}

</style>