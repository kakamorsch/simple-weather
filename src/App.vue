<template>
  <v-app>
    <SimpleWeather :date="obj.date" :temp="obj.temp" :desc="obj.desc" :img="obj.img" />
  </v-app>
</template>

<script>
import SimpleWeather from "./components/SimpleWeather";

export default {
  name: "App",

  components: {
    SimpleWeather
  },

  data: () => ({
    //
    obj: {
      date: "31/05/2020",
      temp: "35º",
      desc: "Predominantemente ensolarado.",
      img: "https://vuejs.org/images/logo.png"
    }
  })
};
</script>
