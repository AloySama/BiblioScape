<template>
  <div class="container">
    <div class="home">
      <h2>Une expérience unique à vivre en équipe !</h2>
    </div>
    <button @click="scrollToAnchorPoint('section1')">Voir les missions !</button>
  </div>
  <div class="boxContainer">
  <div ref="section1" class="games">
    test
  </div>
  <div ref="section1" class="games">
    test
  </div>
</div>
</template>

<script>
export default{
  methods: {
  scrollToAnchorPoint(refName) {
    const el = this.$refs[refName]
    el.scrollIntoView({ behavior: 'smooth'})
  }
}
}
</script>

<style scoped>

/* SCSS des bouttons Post-it */

@import url(https://fonts.googleapis.com/css?family=Permanent+Marker);


.container {
  height: 62vh;
  margin: 0 auto;
  position: relative;
  scroll-behavior: smooth;
}

.boxContainer {
  display: flex;
  flex-direction: row;
}

.games {
  padding-bottom: 20vh;
  width: 300px;
  height: 300px;
  border: 2px solid green;
  padding: 50px;
  margin: 20px;
}

button {
  margin-top: 40px;
  font-size: 40px;
  padding: 20px 60px;
  border-radius: 25px;
  border: none;
  background-color: #42b983;
}

button:hover {
  background-color: darkgreen;
  cursor: pointer;
}


h2, h3 {
  color: chartreuse;
  font-weight: bold;
}

h2, h3 {
  margin-top: 20px;
}

h2 {
  margin-top: 25vh;
  font-size: 50px;
}

h3 {
  font-size: 30px;
}
</style>