<template>

    <!-- Section between the jumbotron and the construction services offered  -->
    <section class="construction-projects-top">
        <h2 class="fw-light">{{sectionContent.title}}</h2>
        <button>{{sectionContent.buttonText}}</button>
    </section>
</template>

<script>

export default {
    name:'ConstructionProjectsTop',
    data() {
        return {
            sectionContent: {
                title: 'Do You Have A Construction Project We Can Help With?',
                buttonText: 'Get a free quote'
            }
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.construction-projects-top {
    display: flex;
    position: relative;
    justify-content: center;
    align-items: center;
    background-color: $vibrantBrightSun;
    height: 130px;

    h2 {
        color: $codGrey;
    }

    button {
        position: absolute;
        bottom: -15px;
        padding: 5px 25px;
        border: 1px solid $primaryWhite;
        background-color: $codGrey;
        color: $primaryWhite;
        text-transform: uppercase;
        font-size: .9rem;

        &:hover {
            color: $codGrey;
            background-color: $primaryWhite;
            border: 1px solid $primaryBlack;
        }

    }

}

</style>