<template>
  <Rain/>
  <!-- <Sun/> -->
  <button @click="toggleRain">Toggle Rain</button>
</template>

<script>
import Rain from './components/Rain.vue'
import Sun from './components/Sun.vue'
export default {
  name: 'App',
  components: {
    Rain,Sun
  },
  data() {
    return {
      toggleRainBool: false
    };
  },
  methods: {
    toggleRain() {
      this.toggleRainBool = !this.toggleRainBool;
    }
  }
}
</script>

