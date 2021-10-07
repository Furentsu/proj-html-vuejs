<template>

  <!-- Section containing the the statistics regarding the services offered  -->
    <section class="container-flex">
        <div class="row">
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
                    icon: 'fas fa-building',
                    number: '3534',
                    title: 'Planning Applications',
                
                },
                {   
                    icon: 'fas fa-sync-alt',
                    number: '896',
                    title: 'Completed Projects',
                
                },
                {   
                    icon: 'fas fa-home',
                    number: '172',
                    title: 'Trained Professionals',
                
                },
                {   
                    icon: 'fas fa-truck',
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
    border: 2px solid black;

    height: 350px;
}

</style>