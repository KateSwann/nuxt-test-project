<template>
  <section class="container">
    <nuxt-link to="/users">Users</nuxt-link>

    <map-loader 
      :map-config="mapConfig"
      apiKey="AIzaSyCdsCZwgVbKBnvwqtPQ8Mqcv5P0lNzuxs8"
    >
      <template v-for="marker in markers">
        <child-marker :position="marker" />
      </template>
    </map-loader>


  </section>
</template>


<script>
import MapLoader from "./MapLoader.vue"
import ChildMarker from './ChildMarker'

export default {
  props: {
    markers: Array
  },
  data(){
    return {
      mapConfig: {
        zoom: 12
      }
    }
  },
  components: {
    MapLoader,
    ChildMarker
  }
}
</script>



<style>
.yamap {
  height: 80vh;
}

.container {
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

