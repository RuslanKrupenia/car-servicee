<template>
<div id="app">
  <Header />
  <About/>
  <Profit/>
  <Services/>
  <ReviewSection/>
  <Works/>
  <FeedbackForm/>
  <!-- <MapComponent/> -->
  
</div>
</template>

<script>
import Header from './components/Header';
import About from './components/About';
import Profit from './components/Profit';
import Services from './components/Services'
import ReviewSection from './components/ReviewSection.vue'
import Works from './components/Works.vue'
import FeedbackForm from './components/FeedbackForm.vue'
// import MapComponent from './components/MapComponent.vue'


export default {
  name: 'App',
  components: {
    Header,About,Profit,Services,Works,FeedbackForm,ReviewSection,
    // MapComponent
  }
}
</script>

<style>

</style>
