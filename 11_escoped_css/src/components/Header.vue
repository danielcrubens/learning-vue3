<template>
  <div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Projeto</a></li>
      <li><a href="#">Contato</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name:'Header'
}
</script>
<style scoped>
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