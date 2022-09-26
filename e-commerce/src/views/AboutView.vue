<script setup>
  const contador2 = {
    data() {
      return {
        contador2 : 0
      }
    },
    mounted() {
      setInterval(() => {
        this.contador2 ++;
      }, 1000)
    }
  }
  let mountedApp = Vue.createApp(contador2).mount('#app')
</script>


<template>
  <div class="about">
    <h1>This is an about page</h1>
    <div id="app2">
      Contador: {{contador}}
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
#app2 {
  font-size: 40px;
  margin-left: 10px;
}
</style>
