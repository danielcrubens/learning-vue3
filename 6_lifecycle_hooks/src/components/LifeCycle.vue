<template>
  <div>
    <h1>Meu nome é: {{nome}}</h1>
  </div>
</template>

<script>
export default{
  name:'LifeCycle',
  data() {
    return {
      nome:'Ainda não sei'
    }
  },
  created(){
    setTimeout(()=>{
      this.nome ='Daniel'
    },1000)
  },
  mounted(){
    setTimeout(()=>{
      this.nome ='Felipe'
    },2000)  }
}
</script>