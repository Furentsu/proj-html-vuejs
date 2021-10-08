<template>

    <!-- Card element  -->
    <div class="card col-6">
        <h2 class="fw-light">Our Home Owners Say</h2>
        <div class="line"></div>
        <div class="image-container">
            <img :src="card[currentIndex].image" alt="Owner image">
        </div>
        <p>{{card[currentIndex].text}}</p>
        <span>{{card[currentIndex].name}}</span>
    </div>
</template>

<script>

export default {
    name:'SliderCard',
    props: {
        card: Array,
    },
    data() {
        return {
            currentIndex: 0,
        }
    },
    mounted() {
        setInterval(() => {
            this.currentIndex++;
            if (this.currentIndex > this.card.length - 1) {
                this.currentIndex = 0;
            }
        }, 5000)
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.card {
    border: none;
    background-color: transparent;
    
    h2 {
        color: $primaryWhite;
    }

    .line {
        height: 2px;
        width: 30%;
        margin: 20px auto;
        background-color: $vibrantBrightSun;
    }

    .image-container {
        width: 100px;
        margin: auto;

        img {
            width: 100%;
            object-fit: cover;
            border-radius: 50%;
        }
    }

    p {
        color: $primaryWhite;
        padding: 30px 0 5px;

    }

    span {
        color: $primaryWhite;
        padding: 20px 0;
    }
    
}

</style>