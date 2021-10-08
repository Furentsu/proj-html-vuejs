<template>

    <!-- Card element  -->
    <div class="card col">
        <div class="logo-container">
            <img :src="content.logo" alt="Partner's logo">
        </div>
    </div>
</template>

<script>

export default {
    name:'TrustedPartnersCard',
    props: ['content']
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.card {
    width: 15%;
    border: none;
    height: 200px;

    .logo-container {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;

        img{
            width: 70%;
        }
    }

}

</style>