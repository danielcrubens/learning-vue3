<template>
  <div>
    <h1> Meu Formulário</h1>
    <form action="" @submit.prevent="enviarFormulario">

      <div>
        <input type="text" v-model="name">
      </div>
      <div>
        <input type="text" v-model="email">
      </div>
      <div>
        <Submit />
      </div>
    </form>
  </div>
</template>

<script>
import InputText from './form/InputText.vue'
import Submit from './form/Submit.vue'
export default {
  name: 'Form',
  components: {
    InputText,
    Submit
  },
  data() {
    return {
      name:'',
      email:''
    }
  },
  methods: {
    enviarFormulario(){
     
      const name = this.name;
      const email = this.email
      console.log('formulário enviado!')
      console.log(`O nome é: ${name}`)
      console.log(`O e-mail é ${email}`)
      
    }
  },
}
</script>