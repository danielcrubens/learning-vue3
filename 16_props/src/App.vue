<template>
  <div>
    <Header :esta_logado="true" />
    <Info/>
    <Pessoa/>
  </div>
</template>
<script>

import Info from './components/Info';
import Pessoa from './components/Pessoa';
import Header from './components/Header.vue';




export default {
  name: 'App',
  components: {
    Info,
    Pessoa,
    Header
  },
  
}
</script>