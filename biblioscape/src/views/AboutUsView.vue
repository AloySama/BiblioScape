<template>
  <div class="ourStory">
    <h1 class="ourProject">Notre projet</h1>
    <p class="ourProjectText">La fréquentation des bibliothèques baisse depuis plusieurs années nous voulons redonner un élan à cette structure et même changer l’avis générale (changer les idées reçus) et <br>
      mettre en lumière les connections entre les deux pays frontaliers.<br><br>
      Notre problématique est donc : <br>
      Comment ré-intéresser la jeunesse à la culture et au patrimoine ?<br>Notre solution « Biblioscape »
      Un concept révolutionnaire d’escape Game au sein d’une bibliothèque, afin de réconcilier la jeunesse avec la lecture tout en leur permettant de découvrir l’histoire <br>
      et la culture Franco-Italienne de façon ludique.</p>
  </div>
  <div class="ourTeam">
    <h1>Notre équipe</h1>
  </div>
  <div class="main">
    <div v-for="user in team" :key="user" class="profile-card">
      <div class="img">
        <img :src="user.img" alt="Team photo">
      </div>
      <div class="caption">
        <h3>{{user.name}}</h3>
        <p>{{user.role}}</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import {defineComponent} from 'vue';

export default defineComponent({
  name: 'ABoutUsView',
  data() {
    return {
      team: [
        {
          name: "Elisa Souchois",
          img: require("../assets/profilPictures/elisa.png"),
          role: "Développeuse"
        },
        {
          name: "Aloïs Brengard",
          img: require("../assets/profilPictures/alois.png"),
          role: "Développeur"
        },
        {
          name: "Julien Prudhomme",
          img: require("../assets/profilPictures/julien.png"),
          role: "Développeur"
        },
        {
          name: "Noah Lahrichi",
          img: require("../assets/profilPictures/noah.png"),
          role: "Graphiste"
        },
        {
          name: "Yohan Vavasseur",
          img: require("../assets/profilPictures/yohan.png"),
          role: "Graphiste"
        },
        {
          name: "Damien (LE BOCAL)",
          img: require("../assets/profilPictures/user.png"),
          role: "Figurant"
        },
      ]
    }
  }
});
</script>


<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.ourTeam {
  margin-top: 6%;
}
.ourProjectText, .ourProject{
  color:  white;
}
.ourStory {
  background-color: black;
}

.ourProject {
  margin-top: 2%;
  margin-bottom: 2%;
}

.main {
  width: 100%;
  height: 350px;
  display: flex;
  justify-content: center;
  align-items: center;
  /* background-color: #0c5db9; */
}

.profile-card {
  position: relative;
  font-family: sans-serif;
  width: 220px;
  height: 220px;
  background: #fff;
  padding: 30px;
  border-radius: 50%;
  box-shadow: 0 0 22px #3336;
  transition: .6s;
  margin: 15px;
  justify-content: space-between;
}

.profile-card:hover {
  border-radius: 10px;
  height: 260px;
}

.profile-card .img {
  position: relative;
  width: 100%;
  height: 100%;
  transition: .6s;
  z-index: 99;
}

.profile-card:hover .img {
  transform: translateY(-60px);
}

.img img {
  width: 100%;
  border-radius: 50%;
  box-shadow: 0 0 22px #3336;
  transition: .6s;
}

.profile-card:hover img {
  border-radius: 10px;
}

.caption {
  text-align: center;
  transform: translateY(-80px);
  opacity: 0;
  transition: .6s;
}

.profile-card:hover .caption {
  opacity: 1;
}

.caption h3 {
  font-size: 21px;
  font-family: sans-serif;
}

.caption p {
  font-size: 15px;
  color: #0c52a1;
  font-family: sans-serif;
  margin: 2px 0 9px 0;
}

.caption .social-links a {
  color: #333;
  margin-right: 15px;
  font-size: 21px;
  transition: .6s;
}

.social-links a:hover {
  color: #0c52a1;
}
</style>