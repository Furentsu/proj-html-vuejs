<template>

    <!-- Section between the jumbotron and the construction services offered  -->
    <section class="construction-projects-top">
        <h2>{{sectionContent.title}}</h2>
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
    border: 2px solid black;

    display: flex;
    position: relative;
    justify-content: center;
    align-items: center;
    height: 130px;

    button {
        position: absolute;
        bottom: -15px;
    }

}

</style>