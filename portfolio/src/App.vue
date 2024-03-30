<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/Footer.vue'
import Header from './components/Header.vue'

</script>

<template>
    <header>
        <Header />
    </header>
      <div class="wrapper">
        <HelloWorld msg="ANNA MAE MONTECALVO" />
        <img src="@/components/icons/anna.jpg" alt="Photo of Anna Mae" class="profile">
      </div>


    <footer>
      <Footer />
    </footer>

  </template>




<style scoped>
header {
  line-height: 1.5;
}

.profile {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}

</style>
