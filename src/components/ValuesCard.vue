<template>

    <!-- Card element  -->
    <div class="card col-2">
        <div class="icon-container" :class="content.bg">
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

.bali-hai {
    background-color: $baliHai;
}

.ship-cove {
    background-color: $shipCove;
}

.orange {
    background-color: $orange;
}

.olive {
    background-color: $olive;
}

.card {
    border: none;
    padding: 20px;
    background-color: transparent;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .icon-container {
        width: 80px;
        height: 80px;
        padding: 40px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 50%;
        
        i {
            font-size: 2.5rem;
            color: $primaryWhite;
        }
    }

    h2 {
        font-size: .9rem;
        padding: 10px 0;
        color: $doveGrey;
    }

    p {
        font-size: .9rem;
        color: $doveGrey;
    }

}

</style>