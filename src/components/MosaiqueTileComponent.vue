<template>
  <div class="tile">
    <div class="tile-img">
      <div>
        <img :src="image" :alt="alt" />
      </div>
    </div>
    <div class="tile-text">
      <h3>{{ title }}</h3>

    </div>
  </div>
</template>

<script>
export default {
  name: "MosaiqueTileComponent",
  props: {
    image: {
      type: String,
      required: true
    },
    alt: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
  }
}
</script>

<style scoped>
  .tile {
    padding-block: 3rem;
    padding-left: 3rem;
    background: #efefef;
  }
  .tile-img{
    min-height: 250px;
    display: flex;
    align-items: center;
  }

  h3{
    font-size: 1.2rem;
    font-weight: 700;
    margin-block: 1rem;
  }
</style>