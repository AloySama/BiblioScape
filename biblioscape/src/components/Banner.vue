<template>
  <section>
    <div class="container">
      <header>
        <div class="left">
          <a href="http://localhost:8081/#/"><img src="../assets/logo.png" alt="logo" width="80" height="80"></a>
        </div>
        <div class="middle">
          <img src="../assets/BiblioScapeLogo.png" height="100" width="209">
        </div>
        <div class="right">
          <nav>
            <router-link v-for="item in list" :key="item" :to="item.to">{{item.name}}</router-link>
          </nav>
        </div>
      </header>
    </div>
  </section>
</template>

<script>
export default {
  name: "Banner-app",
  data() {
    return {
      list: [
        {
          name: "Qui sommes nous ?",
          to: "/aboutUs"
        },
        {
          name: "Accueil",
          to: "/"
        }]
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  text-decoration: none;
}

.middle {
  margin-left:130px;
}

section .container {
  max-width: 1100px;
  margin: 0 auto;
  padding-top: 5px;
  padding-bottom: 5px;
  /* background-color: #f8f7f6; */
  border-bottom-right-radius: 30%;
  border-bottom-left-radius: 30%;
}

section .container header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

section .container nav {
  display: flex;
  flex-direction: row;
  align-items: center;
}

section .container nav a {
  margin-left: 10px;
}

section .container a:nth-child(2) {
  border: 2px solid black;
  padding: 10px 20px;
  border-radius: 20px;
}

</style>

