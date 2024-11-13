<script setup>

import TheWelcome from './components/TheWelcome.vue'
import logo1 from '/logo1.png';
import logo2 from '/logo2.png';
import CannelleGarcia from '/CannelleGarcia.png';

</script>

<template>
  <header>
    <img alt="Vue logo" class="logo1" src="../public/logo1.png"/>
    <img alt="Vue logo" class="logo2" src="../public/logo2.png"/> 
    
  </header>

  <main>
    <TheWelcome />
  </main>



</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 1rem;
}

@media (min-width: 1024px) {
  header {
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo1
{
  /* margin: 1rem 0; */
  width : 100%;
  height : auto;
  display: block;
  margin: 0 auto 1rem;
}

.logo2
{
  /* margin: 1rem 0; */
  width : 50%;
  height : auto;
  display: block;
  margin: 0 auto 1rem;
}

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  } 
}
</style>




