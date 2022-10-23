<template>
  <div class="container">
    <div class="home">
      <h2>Une expérience unique à vivre en équipe !</h2>
    </div>
    <button @click="scrollToAnchorPoint('section1')">Voir les missions !</button>
  </div>
  <div class="boxContainer">
    <div ref="section1" class="box1">
      <div class="card">
        <div class="img1Container"><img src="../assets/test.jpg" class="imgBox1"></div>
        <div class="container">
    <Lorem><br>Lorem ipsum dolor sit amet, consectetur adipiscing elit. <br>Suspendisse ultrices nulla eu rhoncus rutrum.</Lorem> 
  </div>
</div>
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

.img1Container {
  width: 135%;
  margin-top: -50px;
  margin-left: -50px;

}
.imgBox1 {
  width: 100%;
  /* background-color: #f8f7f6; */
}
.boxContainer {
  display: flex;
  flex-direction: row;
  margin-left: 15%;
}

.box1, .box2 {
  padding-bottom: 20vh;
  width: 290px;
  height: 300px;
  border: 2px solid rgb(0, 0, 0);
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