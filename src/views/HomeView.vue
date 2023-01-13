<script>
import HeaderComponent from "../components/HeaderComponent.vue";
import Hero from "../components/Hero.vue";
import SectionOne from "../components/SectionOne.vue";

export default {
  name: "HomeView",
  components: {SectionOne, HeaderComponent, Hero},
  created() {
    document.title = "Alexandre Velia, développeur web freelance";
  }
}
</script>

<template>
  <main>
    <div class="container">
      <HeaderComponent />
      <SectionOne />
    </div>
      <Hero />
  </main>
</template>
