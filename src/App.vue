<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <Card theme="first">
    <template v-slot:img>
       <img src="./assets/icon-sedans.svg" alt="icon-luxury">
    </template>
    <template v-slot:title>
      sedands
    </template>

      <template v-slot:text>
       Choose a sedan for its affordability and excellent fuel economy. Ideal for cruising in the city 
        or on your next road trip.
    </template>
  </Card>

   <Card theme="second">
       <template v-slot:img>
       <img src="./assets/icon-suvs.svg" alt="icon-suvs">
    </template>
    <template v-slot:title>
      SUVs
    </template>

      <template v-slot:text>
      Take an SUV for its spacious interior, power, and versatility. Perfect for your next family vacation 
       and off-road adventures.
    </template>
   </Card>
    <Card theme="third">
            <template v-slot:img>
       <img src="./assets/icon-luxury.svg" alt="icon-suvs">
    </template>
    <template v-slot:title>
      Luxury
    </template>

      <template v-slot:text>
     Cruise in the best car brands without the bloated prices. Enjoy the enhanced comfort of a luxury 
       rental and arrive in style.
    </template>
    </Card>

    <section class="attribution">
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    Coded by <a href="#">Denis B.</a>.
  </section>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Card from './components/CarCard.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Card
  },
  data () {
    return {
      img:['./assets/icon-luxury.svg', '../assets/icon-luxury.svg', '../assets/icon-luxury.svg']
    }
  }
}
</script>

<style>
@import '../src/assets/css/style.css';

.sale {
    background: fuchsia;
    color:white;
}

</style>
