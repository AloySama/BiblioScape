<template>
  <div class="réservation">
    <h1><u>Escape game du moment </u></h1>
    <h2>accessibilités</h2>
    <h4>Cet escape game est disponible ene plusieurs langues notamment : <br>
      - Italien 🇮🇹 <br>
      - Français 🇫🇷 <br>
      - Anglais 🇺🇸 </h4>

  </div>
  <input v-model="date" type="date"/>
  <div v-if="date">
    <div v-for="hour in hours" :key="hour">
    <input  type="radio" :id="hour" name="dateTime">
      <label :for="hour">{{hour}}</label>
    </div>
  </div>
</template>

<script lang="ts">
import {defineComponent} from 'vue';

export default defineComponent({
  data() {
    return {
      date: null,
      hours: ["15", "16h30", "17h"]
    }
  },
  name: 'ReservationComponent',
  props: {
    msg: String,
  },
});
</script>
