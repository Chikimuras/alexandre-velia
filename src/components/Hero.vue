<template>
<div id="hero">
  <div class="hero-content">
    <h2>Développer un meilleur futur pour les professionnels et les particuliers</h2>
    <p>Ma mission est de vous aider à développer votre entreprise et à vous accompagner dans votre projet de création de site web.</p>
    <a class="button" href="mailto:alexandre.m.velia@gmail.com"><span>Me contacter</span></a>
  </div>

</div>
</template>

<script>
export default {
  name: "Hero"
}
</script>

<style scoped>
#hero{
  background: url("../assets/image 7.png") no-repeat center center;
  background-size: cover;
  padding-block: 8rem;
  width: 100%;
  margin-top: 8rem;
}

.hero-content{
  max-width: 50%;
  margin: 0 auto;
  text-align: center;
}

.hero-content p{
  line-height: 1.5em;
  max-width: 65%;
  margin-inline: auto;
  margin-bottom: 2rem;
}
</style>