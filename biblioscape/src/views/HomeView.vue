<template>
  <div class="container">
    <div class="home">
      <h2>Une expérience unique à vivre en équipe !</h2>
    </div>
    <button @click="scrollToAnchorPoint('section1')">Voir les missions !</button>
  </div>
  <div class="test">
  <div class="boxContainer">
      <div ref="section1" class="box1">
        <div class="card">
          <div class="img1Container"><img src="../assets/Fond_guerre.png" class="imgBox1"></div>
          <div class="boxText">
            <Lorem>Le jeu se déroule durant la seconde guerre mondiale vous incarnez une unité de soldat mené par le colonel Francisco, à la suite d’un largage de bombe vous vous retrouvez coincer dans une mystérieuse bibliothèque ou les livres relatent à la fois du passé et du futur !
              Pour vous sortir de là vous devrez chercher à travers les nombreux livres et déchiffrer
              le code pour mettre fin à cette guerre.
            </Lorem><br><br>
            Réservation <router-link to="/reservation">ici</router-link>
          </div>
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

a {
  color: white;
}

.boxText {
  margin-left: -50px;
  font-size: 15px;
  margin-top: -5px;
  width: 134%;
  text-align: justify;
}

.container {
  height: 62vh;
  margin: 0 auto;
  position: relative;
  scroll-behavior: smooth;
}

.test {
  overflow: scroll;
  background: url("../assets/Fondblur.png");
  padding-bottom: 50vh;
}

.img1Container {
  width: 135%;
  margin-top: -50px;
  margin-left: -50px;

}
.imgBox1 {
  width: 100%;
  height: 270px;
  /* background-color: #f8f7f6; */
}
.boxContainer {
  display: flex;
  flex-direction: row;
  margin-left: 15%;
}

.box1, .box2 {
  background-color: #333333;
  color: #42b983;
  width: 290px;
  height: 350px;
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