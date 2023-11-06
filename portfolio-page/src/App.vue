<template>
  <div>
    <Navbar />
    <MyPortfolio />
  </div>
</template>

<script setup>
import MyPortfolio from './components/MyPortfolio.vue'
import Navbar from './components/Navbar.vue'
</script>

<style>

#app{
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #edfff3;
}
body {
  display: flex;
  margin: 0;
  overflow-x: hidden;
}
</style>
