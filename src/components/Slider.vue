<template>
    <section class="slider d-flex justify-content-center align-items-center container-flex">
        <div class="row d-flex justify-content-center text-center">
            <SliderCard :card="cardsContent"/>
        </div>

        <!-- <nav>

        </nav> -->

    </section>
</template>

<script>
import SliderCard from './SliderCard.vue'

export default {
    name: 'Slider',
    components: {
        SliderCard
    },
    data() {
        return {
            cardsContent: [
                {   
                    image: require('../assets/images/home-testimonial-113165296.jpg'),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae optio unde deserunt obcaecati consectetur error ratione soluta natus ut dignissimos perspiciatis totam molestiae sit sapiente odio, dolore fugit numquam sed.',
                    name: 'Megan Robinson - New Home Owner'
                },
                {   
                    image: require('../assets/images/home-testimonial-84268399.jpg'),
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo laudantium soluta quidem nostrum totam recusandae, facilis voluptatum deleniti vitae voluptatibus dolorum. Voluptatem dicta in eligendi illo aperiam exercitationem quia perspiciatis.',
                    name: 'Harry Smith - Home Owner'
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

.slider {
    height: 500px; 
    background-image: url('../assets/images/home-parallax-144609983.jpg');
    background-size: cover;
    background-position: center;

}

</style>