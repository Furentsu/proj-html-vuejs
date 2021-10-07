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
    border: 1px solid red;
    
    height: 200px;

    .logo-container {
        width: 100%;

        img{
            width: 100%;
        }
    }

}

</style>