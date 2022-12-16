<template>
  <div>
    <PrimeiroComponente/>
  </div>
</template>
<script>

import Reutilizacao from './components/Reutilizacao.vue';
import PrimeiroComponente from './components/PrimeiroComponente.vue';




export default {
  name: 'App',
  components: {
    Reutilizacao,
    PrimeiroComponente
  },
  
}
</script>