<script>
import HeaderComponent from "../components/HeaderComponent.vue";
import Hero from "../components/Hero.vue";

export default {
  name: "HomeView",
  components: {HeaderComponent, Hero},
  created() {
    document.title = "Alexandre Velia, développeur web freelance";
  }
}
</script>

<template>
  <main>
    <div class="container">
      <HeaderComponent />
    </div>
      <Hero />
  </main>
</template>
