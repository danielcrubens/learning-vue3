<template>
  <div>
  <LifeCycle />
  <Pessoa/>
</div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from'./components/Pessoa.vue'

export default {
  name: 'App',
  components: {
    LifeCycle,
    Pessoa
  },
  data() {
    return {
    }
  },
}
</script>