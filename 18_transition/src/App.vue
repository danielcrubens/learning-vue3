<template>
  <button @click="show = !show">Toggle</button>

  <transition name="fade">
    <h1 v-if="show">Front-end</h1>
  </transition>

	<transition name="scale">
    <h1 v-if="show">Front-end</h1>
  </transition>

</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  data() {
    return {
      show: false
    }
  },
})
</script>

<style scoped>

/* 
v-enter-from (de onde estar vindo)
v-enter-active (como vai acontecer)
v-enter-to (para onde está indo)

v-leave-from (de onde estar vindo)
v-leave-active (como vai acontecer)
v-leave-to (para onde está indo)

O nome inicial `v` depende do atributo `name`
*/

.fade-enter-from,
.fade-leave-to{
opacity: 0;
}

.fade-enter-active,
.fade-leave-active{
transition: opacity 0.5s;
}
</style>