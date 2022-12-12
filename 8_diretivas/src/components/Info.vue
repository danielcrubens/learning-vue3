<template>
  <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
  <p v-else>Estou em busca de novas oportunidades!</p>

  <p v-show="mostrar_email">Mande uma mensagem para: dcr.tecnologi@gmail.com</p>
</template>
<script>
export default {
  name: 'Info',
  data() {
    return { 
      esta_trabalhando: false,
      mostrar_email: false
    }
  }
}
</script>