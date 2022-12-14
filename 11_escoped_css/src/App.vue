<template>
  <Header/>
  <div>
    <LifeCycle/>
    <Info/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import LifeCycle from './components/LifeCycle.vue';
import Info from './components/Info';


export default {
  name: 'App',
  components: {
    LifeCycle,
    Info,
    Header
  },
  data() {
    return {
    }
  },
}
</script>
<style>
body{
  background-color: #333;
  color:#fff;
}
</style>