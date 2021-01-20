<template>
  <div id="app">
    {{count}}
    {{$store.getters.doubleCount}}
    <!-- <button @click="$store.commit('increment')">count++</button> -->
    <button @click="$store.dispatch('increment2')">count++</button>
  </div>
</template>

<script>

export default {
  name: 'App',
  computed:{
    count(){
      return this.$store.state.count
    }
  }
  
}
</script>

<style>

</style>
