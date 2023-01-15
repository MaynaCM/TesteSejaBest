
<template>
  <div class="h-screen columns-2 grid-cols-2 gap-2 bg">
    <div class="h-full w-full flex">
      <h1 class="text-5xl text-white self-center ml-20 font-bold animate__fadeInLeft">Bem vindo!<br>Faça seu Cadastro ao lado!</h1>    
    </div>
    <base-form />
  </div>
 
</template>

<style>
</style>

<script>
import BaseForm from './components/teste.vue'
export default {
    name: "app",
    components: {
      BaseForm
    }

  }
</script>
