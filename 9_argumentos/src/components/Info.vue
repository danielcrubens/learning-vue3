<template>
  <p>Para acessar me portfólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
  <Picture />
</template>

<script>
import Picture from './Picture.vue'
export default {
  name: 'Info',
  components:{
    Picture
  },
  data() {
    return { 
      esta_trabalhando: false,
      mostrar_email: false,
      meu_link:'https://danielcrubens.github.io'
    }
  }
}
</script>