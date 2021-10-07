<template>

  <!-- Section containing the the statistics regarding the services offered  -->
    <section class="container-flex">
        <div class="row d-flex justify-content-center">
            <StatisticsCard v-for="(element,index) in cardsContent" :key="index" :content="element" />
        </div>
    </section>
</template>

<script>
import StatisticsCard from './StatisticsCard.vue'


export default {
name:'Statistics',
    components: {
        StatisticsCard,
    },
    data() {
        return {
            cardsContent: [
                {   
                    icon: 'far fa-paper-plane',
                    number: '3534',
                    title: 'Planning Applications',
                
                },
                {   
                    icon: 'far fa-building',
                    number: '896',
                    title: 'Completed Projects',
                
                },
                {   
                    icon: 'fas fa-users',
                    number: '172',
                    title: 'Trained Professionals',
                
                },
                {   
                    icon: 'fas fa-globe',
                    number: '19',
                    title: 'International Offices',
                
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section {
    border: 1px solid black;
    
    padding: 100px;
    height: 450px;
    background-image: url('../assets/images/home-244125289.jpg');
    background-size: cover;

}

</style>