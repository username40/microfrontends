<template>
  <LMap class="map" :zoom="zoom" :center="center">
    <LTileLayer :url="url"></LTileLayer>
    <LCircle
        :lat-lng="circle.center"
        :radius="circle.radius"
        :color="circle.color"
    />
  </LMap>
</template>

<script>
import "leaflet/dist/leaflet.css"
// eslint-disable-next-line no-unused-vars
import L from 'leaflet';
import {LMap, LTileLayer, LCircle} from 'vue2-leaflet';
export default {
  name: "Map",
  components: {
    LMap,
    LTileLayer,
    LCircle
  },
  data() {
    return {
      url: 'https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
      zoom: 12,
      center: [68.968195, 33.074843],
      circle: {
        center: [68.968195, 33.074843],
        radius: 555,
        color: 'red'
      }
    }
  }
}
</script>

<style scoped>
.map {
  width: 100%;
  height: 400px
}
</style>