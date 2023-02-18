<template>
  <div id="header">
    <div class="intro-block">
      <h1 class="intro-lead-in">Développeur web full-stack</h1>
      <p class="intro-text">De la conception jusqu'à la mise en production, mon expertise et mon savoir-faire dans le domaine du web me permettront de vous accompagner dans chacun des processus de votre projet.</p>
      <a class="button" href="/portfolio"><span>En savoir +</span></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent"
}
</script>

<style scoped>
#header {
  background: url("../assets/Home-10-rev-img 1.png") no-repeat center right;
  background-size: 50%;
  padding-block: 10rem;
}

.intro-block {
  max-width: 50%;
}

.intro-lead-in {
  line-height: 1em;
  margin-bottom: 2rem;
}

.intro-text{
  line-height: 1.5em;
  max-width: 65%;
  margin-bottom: 5rem;
}
</style>