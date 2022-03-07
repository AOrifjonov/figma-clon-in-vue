<script setup>
import Navbar from './components/navbar/Navbar.vue'
import LeftPanel from './components/fixed/LeftPanel.vue'
import NavbarBottom from './components/fixed/NavbarBottom.vue'
import SecondNavBottom from './components/fixed/SecondNavBottom.vue'
import Recent from './components/main/Recent.vue'
</script>

<template>
  <Navbar />
  <LeftPanel />
  <NavbarBottom />
  <SecondNavBottom />
  <Recent />
</template>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  font-family: sans-serif;
}

</style>
