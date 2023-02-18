<template>
  <div class="section2">
    <div class="section2-title">
      <h2>{{ title }}</h2>
    </div>
    <div class="section2-content">
      <Dropcap
          title="Création d’outils sur mesure"
          side="right"
          text="Après avoir défini les besoins de votre entreprise. Je réalise en accord avec le cahier des charges un ERP sur mesure tailler pour VOTRE entreprise."
          :image="image1"
          number="01"
      />
      <Dropcap
          title="Développement multi-plateforme"
          side="left"
          text="En plus d’application web parfaitement sur mesure. Une application mobile ou tablette peut être le complément idéal. Selon l’utilisation et les besoins de multiples options seront possible."
          :image="image2"
          number="02"
      />
      <Dropcap
          title="Conception d’application pour les pros"
          side="right"
          text="Fils et petit-fils d’artisan, je me suis naturellement spécialisé dans la conception d’outils pour les professionnels du secteur secondaire et primaire."
          :image="image3"
          number="03"
      />
      <Dropcap
          title="Sites web & e-commerces modernes et performants"
          side="left"
          text="Afin de vous permettre une visibilité grandissante sur le web, je mets à votre service mes compétences de développement web pour vous proposer des sites sur mesure, modernes et performants."
          :image="image4"
          number="04"
      />
    </div>
  </div>
</template>

<script>
import Dropcap from "./Dropcap.vue";
import image1 from "../assets/dropcap-1.png";
import image2 from "../assets/dropcap-2.png";
import image3 from "../assets/dropcap-3.png";
import image4 from "../assets/dropcap-4.png";

export default {
  name: "SectionTwo",
  components: {Dropcap},
  props: {
    title: {
      type: String,
      required: true
    },
  },
  data() {
    return {
      image1: image1,
      image2: image2,
      image3: image3,
      image4: image4
    }
  }
}
</script>

<style scoped>
  .section2-title {
    max-width: 35%;
    margin-inline: auto;
    text-align: center;
  }
</style>