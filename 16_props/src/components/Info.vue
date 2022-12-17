<template>
  <div>
    <button @click="showEmail">{{ textoBotao }}</button>
    <p v-show="mostrar_email">Mande uma mensagem para:{{ email }}</p>
    <p>Utilizo as seguintes tecnologias para back-end: </p>
    <ul>
      <li v-for="(tecnology, index) in  backend_technologies" v-bind:key="index">{{ tecnology }}</li>
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end</p>
    <ul>
      <li v-for="tecnology in frontend_technologies" :key="tecnology.id">{{ tecnology.language }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Info',
  props: {
    email: String,
    esta_trabalhando: Boolean,

  },

  data() {
    return {
      mostrar_email: false,
      meu_link: 'https://danielcrubens.github.io',
      textoBotao: 'Mostrar e-mail',
      backend_technologies: ['JavaScript', 'PHP', 'Python'],
      frontend_technologies: [
        { id: 1, language: 'HTML' },
        { id: 2, language: 'CSS' },
        { id: 3, language: 'Vue' }
      ]
    }
  },
  methods: {
    showEmail() {
      console.log("entrou")
      this.mostrar_email = !this.mostrar_email
      if (!this.mostrar_email) {
        this.textoBotao = 'Mostrar e-mail'
      } else {
        this.textoBotao = 'Esconder e-mail'
      }
    }
  }
}
</script>