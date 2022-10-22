<template>
  <div class="réservation">
    <h1> <u>Escape game du moment </u> </h1>
    <h2>accessibilités</h2>
    <h4>Cet escape game est disponible ene plusieurs langues nottament : <br>
    - Italien 🇮🇹 <br>
    - Français 🇫🇷 <br>
    - Anglais 🇺🇸 </h4>

  </div>
  <div class="Subject">
    <h2><u>Synopsis</u></h2>
    <p>Vous allez vous re</p>
    <input type="date"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ReservationComponent',
  props: {
    msg: String,
  },
});
</script>
