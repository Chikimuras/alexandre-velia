<template>
  <div v-if="side === 'left'" class="dropcap">
    <div class="dropcap-content">
      <div class="dropcap-number">
        <h2>{{ number }}</h2>
      </div>
      <div class="dropcap-text">
        <h2>{{ title }}</h2>
        <p>{{ text }}</p>
      </div>
    </div>
    <div class="dropcap-seperator">
      <div class="line"></div>
      <div class="dot"></div>
    </div>
    <div class="dropcap-image">
      <img :src="image" :alt="title" />
    </div>
  </div>
  <div v-else class="dropcap">
    <div class="dropcap-image">
      <img :src="image" :alt="title" />
    </div>
    <div class="dropcap-seperator">
      <div class="line"></div>
      <div class="dot"></div>
    </div>
    <div class="dropcap-content">
      <div class="dropcap-number">
        <h2>{{ number }}</h2>
      </div>
      <div class="dropcap-text">
        <h2>{{ title }}</h2>
        <p>{{ text }}</p>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: "Dropcap",
  props: {
    number: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    },
    side: {
      type: String,
      required: true,
      default: "left"
    }
  }
}
</script>

<style scoped>
.dropcap{
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
}
.dropcap-content{
  padding-block: 10em;
  position: relative;
  z-index: 1;
}
.dropcap-number{
  z-index: -1;
  position: absolute;
  top: -30%;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  opacity: .2;
}

.dropcap-image{
  display: flex;
  align-items: center;
  justify-content: center;
}

.dropcap-number h2{
  font-size: 20rem;
  font-weight: 300;
  color: #efefef;
  margin: auto;
}
.dropcap-text{
  color: #979797;
}
.dropcap-text h2{
  font-size: 2.18rem;
  font-weight: 600;
  color: #000;
  margin-block: 1rem;
  background: none;
  -webkit-background-clip: initial;
  -webkit-text-fill-color: initial;
  text-align: left;
}
.dropcap-seperator{
  position: relative;
  z-index: 1;
}
.line{
  width: 1px;
  height: 100%;
  background: linear-gradient(90deg, rgba(0,212,255,1) 0%, rgba(173,62,255,1) 100%);
  margin: auto;
}
.dot{
  width: 10px;
  height: 10px;
  background: linear-gradient(90deg, rgba(0,212,255,1) 0%, rgba(173,62,255,1) 100%);
  border-radius: 50%;
  margin: auto;
  position: absolute;
  top: 50%;
  left: calc(50% - 5px);
}
</style>