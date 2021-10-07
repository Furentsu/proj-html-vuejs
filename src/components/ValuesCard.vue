<template>

    <!-- Card element  -->
    <div class="card col-2">
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
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .icon-container {
    border: 1px solid blue;

        width: 80px;
        height: 80px;

        i {
            font-size: 3.5rem;
            color: $primaryWhite;
        }
    }

    h2 {
        font-size: .9rem;
    }

    p {
        font-size: .9rem;
    }
}

</style>