<template>
  <div class="home">
    <h3>Une expérience unique à vivre en équipe !</h3>
    <h4>Nos Escapes Game du moment :</h4>
  </div>
  <div class="group-sticky">
  <div class="pad">
  <h1>1ère Escape Game</h1>
  <span class="peel">
    <span class="peel-back"></span>  
  </span> 
</div>
<div class="pad">
  <h1>2ème Escape Game</h1>
  <span class="peel">
    <span class="peel-back"></span>  
  </span> 
</div>
</div>
</template>

<style>

/* SCSS des bouttons Post-it */

@import url(https://fonts.googleapis.com/css?family=Permanent+Marker);

.group-sticky {
  display: flex;
}
.pad {
  position: relative;
  z-index: 2;
  margin: 0 auto;
  margin-top: 50px;
  width: 40vw;
  height: 60vh;
  background-color: #FFFF66;
  -webkit-box-shadow: 0 -1px 7px 1px #333;
  -moz-box-shadow: 0 -1px 7px 1px #333;
  box-shadow: 0 -1px 7px 1px #333;
  border-bottom: 3px solid #E6E65C;
}
.pad h1 {
  position: absolute;
  z-index: 20;
  left: 20px;
  font-weight: normal;
}
.peel {
  position: absolute;
  z-index: 0;
  bottom: 0;
  right: 0;
  height: 60px;
  width: 60px;
  background-color: #E6E65C;
  -webkit-transition: width 500ms, height 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms;
  -o-transition: width 500ms, height 500ms;
  transition: width 500ms, height 500ms;
}
.peel:hover {
  height: 200px;
  width: 200px;
  -webkit-transition: width 500ms, height 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms;
  -o-transition: width 500ms, height 500ms;
  transition: width 500ms, height 500ms;
}
.peel:hover::before {
  height: 100px;
  width: 200px;
  -webkit-transition: width 500ms, height 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms;
  -o-transition: width 500ms, height 500ms;
  transition: width 500ms, height 500ms;
}
.peel:hover::after {
  height: 200px;
  width: 100px;
  right: 100px;
  -webkit-transition: width 500ms, height 500ms, right 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms, right 500ms;
  -o-transition: width 500ms, height 500ms, right 500ms;
  transition: width 500ms, height 500ms, right 500ms;
}
.peel:hover .peel-back {
  bottom: 17px;
  right: 65px;
  width: 80px;
  height: 155px;
  -webkit-transition: width 500ms, height 500ms, right 500ms, bottom 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms, right 500ms, bottom 500ms;
  -o-transition: width 500ms, height 500ms, right 500ms, bottom 500ms;
  transition: width 500ms, height 500ms, right 500ms, bottom 500ms;
}
.peel::before {
  position: absolute;
  z-index: 5;
  top: 0;
  right: 0;
  content: "";
  height: 31px;
  width: 61px;
  background-color: #FFFF66;
  border-bottom: 1px #B8B84A solid;
  -webkit-border-radius: 0 0 50% 0;
  -moz-border-radius: 0 0 50% 0;
  border-radius: 0 0 50% 0;
  -webkit-transition: width 500ms, height 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms;
  -o-transition: width 500ms, height 500ms;
  transition: width 500ms, height 500ms;
  background: -webkit-gradient(linear, 76% 85%, 82% 100%, from(#FFFF66), to(#B8B84A));
}
.peel::after {
  position: absolute;
  z-index: 6;
  bottom: 0px;
  right: 30px;
  content: "";
  height: 61px;
  width: 31px;
  background-color: #FFFF66;
  -webkit-border-radius: 0 0 50% 0;
  -moz-border-radius: 0 0 50% 0;
  border-radius: 0 0 50% 0;
  -webkit-transition: width 500ms, height 500ms, right 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms, right 500ms, -webkit-transform 500ms;
  -o-transition: width 500ms, height 500ms, right 500ms, -webkit-transform 500ms;
  transition: width 500ms, height 500ms, right 500ms;
  background: -webkit-gradient(linear, 56% 94%, 67% 100%, from(#FFFF66), to(#B8B84A));
}
.peel-back {
  position: absolute;
  z-index: 2;
  bottom: 5px;
  right: 19px;
  width: 20px;
  height: 46px;
  background-color: #CCCC6A;
  transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -webkit-transform: rotate(45deg);
  -webkit-transition: width 500ms, height 500ms, right 500ms, bottom 500ms, -webkit-transform 500ms;
  -moz-transition: width 500ms, height 500ms, right 500ms, bottom 500ms;
  -o-transition: width 500ms, height 500ms, right 500ms, bottom 500ms;
  transition: width 500ms, height 500ms, right 500ms, bottom 500ms;
  -webkit-box-shadow: 0 0 5px 2px #808033;
  -moz-box-shadow: 0 0 5px 2px #808033;
  box-shadow: 0 0 5px 2px #808033;
}
</style>