<template>
  <div>
    <Reutilizacao />
    <h1>Olá Vue!</h1>
    <Reutilizacao />
  </div>
</template>

<script>
import Reutilizacao from './Reutilizacao.vue'

export default {
  name: 'PrimeiroComponente',
  components: {
    Reutilizacao
  },
}
</script>