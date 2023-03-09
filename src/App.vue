<template>
<div id="app">
  <Header />
  <About/>
  <Profit/>
  <Services/>
  <Works/>
  <FeedbackForm/>

</div>
</template>

<script>
import Header from './components/Header';
import About from './components/About';
import Profit from './components/Profit';
import Services from './components/Services'
import Works from './components/Works.vue'
import FeedbackForm from './components/FeedbackForm.vue'


export default {
  name: 'App',
  components: {
    Header,About,Profit,Services,Works,FeedbackForm
  }
}
</script>

<style>

</style>
