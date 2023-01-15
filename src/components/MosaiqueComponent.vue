<template>
  <div id="section-2">
    <div class="grid grid-rows-2 grid-cols-3">
      <div class="col-span-1 row-span-1 flex align-items-center">
        <div class="center-container">
          <p class="pre-title">
            <span class="pre-title__text">Services et suivi</span>
          </p>
          <h2>Des services sur-mesure et un suivis parfait</h2>
          <a class="button"><span>En savoir +</span></a>
        </div>
      </div>
      <div class="col-span-1 row-span-1">
        <MosaiqueTileComponent
          :image="image1"
          :alt="'Outils de gestion d\'entreprise'"
          :title="'Outils de gestion d\'entreprise'"
        />
      </div>
      <div class="col-span-1 row-span-1">
        <MosaiqueTileComponent
            :image="image2"
            :alt="'Conception & conseils'"
            :title="'Conception & conseils'"
        />
      </div>
      <div class="col-span-1 row-span-1">
        <MosaiqueTileComponent
            :image="image3"
            :alt="'Site web & e-commerce'"
            :title="'Site web & e-commerce'"
        />
      </div>
      <div class="col-span-1 row-span-1">
        <MosaiqueTileComponent
            :image="image4"
            :alt="'Maintenance & optimisation'"
            :title="'Maintenance & optimisation'"
        />
      </div>
      <div class="col-span-1 row-span-1">
        <MosaiqueTileComponent
            :image="image5"
            :alt="'Déploiement & bugfixing'"
            :title="'Déploiement & bugfixing'"
        />
      </div>
    </div>
  </div>
</template>

<script>
import MosaiqueTileComponent from "./MosaiqueTileComponent.vue";
import image1 from "../assets/img1.png";
import image2 from "../assets/img2.png";
import image3 from "../assets/img3.png";
import image4 from "../assets/img4.png";
import image5 from "../assets/img5.png";

export default {
  name: "MosaiqueComponent",
  components: {MosaiqueTileComponent},
  data() {
    return {
      image1: image1,
      image2: image2,
      image3: image3,
      image4: image4,
      image5: image5
    }
  }
}

</script>

<style scoped>
#section-2{
  margin-bottom: 5rem;
}
  h2 {
    padding-right: 3rem;
  }
</style>