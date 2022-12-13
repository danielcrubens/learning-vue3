<template>
  <div>
  <button @click="showEmail">{{textoBotao}}</button>
  <p v-show="mostrar_email">Mande uma mensagem para:{{email}}</p>
  </div>
</template>

<script>
export default {
  name: 'Info',

  data() {
    return { 
      esta_trabalhando: false,
      mostrar_email: false,
      meu_link:'https://danielcrubens.github.io',
      email:'dcr.tecnlogi@gmail.com',
      textoBotao:'Mostrar e-mail'
    }
  },
  methods:{
    showEmail(){
      console.log("entrou")
      this.mostrar_email = !this.mostrar_email
      if (!this.mostrar_email) {
        this.textoBotao ='Mostrar e-mail'
      }else{
        this.textoBotao ='Esconder e-mail' 
      }
    }
  }
}
</script>