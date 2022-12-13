<template>
  <div>
    <LifeCycle/>
    <Info/>
  </div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue';
import Info from './components/Info';


export default {
  name: 'App',
  components: {
    LifeCycle,
    Info
  },
  data() {
    return {
    }
  },
}
</script>