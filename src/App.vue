<template>
  <div id="app">
    <landing-page></landing-page>
    <destination-page></destination-page>
    <sale></sale>
    <top-destinations></top-destinations>
    <happy-click></happy-click>
    <footer-comp></footer-comp>
  </div>
</template>

<script>
import Landing from './components/LandingComponent/LandingPage.vue';
import Destinations from './components/GridComponent/DestinationGrid.vue';
import Sale from './components/SaleComponent/Sale.vue';
import TopDestinations from './components/TopComponent/TopDestinations.vue';
import HappyClick from './components/TopComponent/HappyClick.vue';
import Footer from './components/FooterComponent/Footer.vue';

export default {
  components: {
    LandingPage: Landing,
    DestinationPage: Destinations,
    Sale: Sale,
    TopDestinations: TopDestinations,
    HappyClick: HappyClick,
    FooterComp: Footer
  },
  data () {
    return {
      
    }
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro:400,400i,600');

  html, body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Source Sans Pro', sans-serif;
  }

  .intro {
      text-align: center;
      margin: 0 10rem;
      color: #3b3b3b;
      text-shadow: none;
  }

  .intro > h1 {
      text-transform: uppercase;
      letter-spacing: 1.1px;
  }

  .intro > p {
      line-height: 1.5rem;
  }

  hr {
      max-width: 25rem;
  }

</style>
