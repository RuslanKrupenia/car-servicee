<template>
<div id="app">
  <Header />
  <About/>
  <Profit/>
  <Services/>
</div>
</template>

<script>
import Header from './components/Header';
import About from './components/About';
import Profit from './components/Profit';
import Services from './components/Services'


export default {
  name: 'App',
  components: {
    Header,About,Profit,Services
  }
}
</script>

<style>

</style>
