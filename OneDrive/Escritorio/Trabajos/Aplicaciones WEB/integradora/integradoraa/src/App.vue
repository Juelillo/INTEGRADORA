<script setup lang="ts">
import {onMounted, ref} from "vue";
import PageHeader from "./components/PageHeader.vue";
import Carrusel from "./components/carrusel.vue";
import CarruselDos from "./components/carruselDos.vue";
import CarruselTres from "./components/carruselTres.vue";
import BtnUno from "./components/btnUno.vue";
import BtnDos from "./components/btnDos.vue";
import BtnTres from "./components/btnTres.vue";
import Ofertas from "./components/ofertas.vue";
import axiosClient from "./utils/axios";

/*const countries = ref([]);
const fetchCountries = async() => {
  try {
  const {data} = await axiosClient.get("/all");
  countries.value = data;
  } catch (error) {
    console.log(error);
  }
}

onMounted(() => {
  fetchCountries();
})


<div v-for="country in countries">{{ country.name.common }}</div>*/
</script>

<template>
  <PageHeader/>
  <Ofertas/>
  <div>
    <Carrusel/>
    <BtnUno/>
  </div>
  <div>
    <CarruselDos/>
    <BtnDos/>
  </div>
  <div>
    <CarruselTres/>
    <BtnTres/>
  </div>
</template>
