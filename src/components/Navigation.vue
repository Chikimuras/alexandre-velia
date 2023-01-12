<template>
  <header>
    <div>
      <div class="logo">
        <a href="/"><img width="150" src="@/assets/logo.svg" alt="logo" /></a>
      </div>
      <nav>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "navigation"
}
</script>

<style scoped>

</style>