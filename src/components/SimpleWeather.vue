<template>
  <v-content>
    <v-card class="mx-auto" max-width="400" tile>
      <v-list>
        <v-list-item class="date">{{date}}</v-list-item>
        <v-list-item>
          <v-img :src="img" contain></v-img>
        </v-list-item>
        <v-list-item class="temp">{{temp}}</v-list-item>
        <v-list-item class="desc">{{desc}}</v-list-item>
      </v-list>
    </v-card>
  </v-content>
</template>

<script>
export default {
  name: "SimpleWeather",
  data: () => ({}),
  props: ["date", "temp", "desc", "img"]
};
</script>
<style scoped>
.date {
  left: 100px;
  font-size: 30px;
  font-weight: bold;
}
.temp {
  left: 28px;
  font-size: 38px;
  font-weight: bolder;
}
.desc {
  font-size: 22px;
  font-weight: normal;
}
</style>
