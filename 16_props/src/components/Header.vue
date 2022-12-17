<template>
  <div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Projeto</a></li>
      <li><a href="#">Contato</a></li>
      <li v-if="esta_logado"><a href="#">Meu Perfil</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name:'Header',
  props:['esta_logado']
}
</script>
<style scoped>
div{
  background:#000;
  width: 100%;
}
ul{
  list-style-type: none;
  display: flex;
  align-items: center;
  justify-content: center ;
}
li{
  margin-right: 10px;
}
a{
  color: #DDD;
  text-decoration: none;
  transition: .5s;
  font-weight: bold;
}
a:hover{
  color: turquoise;
}

</style>