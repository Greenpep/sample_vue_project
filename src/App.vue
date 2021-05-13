<template>
  <h1>Favorite IU songs library</h1>
  <button @click="songsTrigger" v-if="!showSongs">Show songs</button>
  <Applause v-if="!showSongs" :applause_counter="applause_counter" />
  <button @click="songsTrigger" v-if="showSongs">Hide songs</button>
  <Songs v-if="showSongs" />
</template>

<script>
import Songs from './components/Songs.vue'
import Applause from './components/Applause.vue'
export default {
  name: 'App',
  components: { Songs, Applause },
  data(){
    return{
      showSongs: false,
      applause_counter: 0
    }
  },
  methods: {
    songsTrigger(){
      this.showSongs = !this.showSongs
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
