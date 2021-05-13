<template>
  <h1>Favorite IU songs library</h1>

  <button @click="songsTrigger" v-if="!showSongs">Show songs</button>
  <button @click="songsTrigger" v-if="showSongs">Hide songs</button>
  <button @click="formTrigger" v-if="!showForm">Show fan form</button>
  <button @click="formTrigger" v-if="showForm">Hide fan form</button>

  <Applause v-if="!showSongs && !showForm" :applause_counter="applause_counter" @click="applauseOnce"/>
  <p v-if="!showSongs && !showForm"> Applause Counter: {{ this.applause_counter }} </p>
  <Songs v-if="showSongs" />
  <Form v-if="showForm" />
</template>

<script>
import Songs from './components/Songs.vue'
import Applause from './components/Applause.vue'
import Form from './components/Form.vue'
export default {
  name: 'App',
  components: { Songs, Applause, Form },
  data(){
    return{
      showSongs: false,
      showForm: false,
      applause_counter: 0
    }
  },
  methods: {
    songsTrigger(){
      this.showSongs = !this.showSongs
    },
    formTrigger(){
      this.showForm = !this.showForm
    },
    applauseOnce(){
      this.applause_counter++
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
}
body{
  margin: 0;
  background:rgb(255, 237, 212)
}
</style>
