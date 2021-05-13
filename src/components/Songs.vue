<template>
  <div class="songs">
      <div class="song_sample" @click="triggerFavorite1" v-bind:style=" {'background-color': actual_color1} ">
          <img :src="lilac" :alt="lilac_img">
          LILAC
      </div>
      <div class="song_sample" @click="triggerFavorite2" v-bind:style=" {'background-color': actual_color2}">
          <img :src="celebrity" :alt="celebrity_img">
          Celebrity
      </div>
      <div class="song_sample" @click="triggerFavorite3" v-bind:style=" {'background-color': actual_color3}">
          <img :src="good_day" :alt="good_day_img">
          Good Day
      </div>
      <div class="song_sample" @click="triggerFavorite4" v-bind:style=" {'background-color': actual_color4}">
          <img :src="you_and_i" :alt="you_and_i_img">
          You And I
      </div>
      <div class="song_sample" @click="triggerFavorite5" v-bind:style=" {'background-color': actual_color5}">
          <img :src="bbibbi" :alt="bbibbi_img">
          BBIBBI
      </div>
      <div class="song_sample" @click="triggerFavorite6" v-bind:style=" {'background-color': actual_color6}">
          <img :src="palette" :alt="palette_img">
          Palette
      </div>
      <div class="song_sample" @click="triggerFavorite7" v-bind:style=" {'background-color': actual_color7}">
          <img :src="eight" :alt="eight_img">
          eight
      </div>
      <div class="song_sample" @click="triggerFavorite8" v-bind:style=" {'background-color': actual_color8}">
          <img :src="blueming" :alt="blueming_img">
          Blueming
      </div>
      <div class="song_sample" @click="triggerFavorite9" v-bind:style=" {'background-color': actual_color9}">
          <img :src="nslcb" :alt="nslcb_img">
          Not Spring, Love, or Cherryblossom
      </div>
  </div>
</template>

<script>
import lilac from '../assets/LILAC.jpeg'
import celebrity from '../assets/Celebrity.jpg'
import good_day from '../assets/Good_Day.png'
import you_and_i from '../assets/You&I.jpg'
import bbibbi from '../assets/bbibbi.jpg'
import palette from '../assets/Palette.png'
import eight from '../assets/eight.jpg'
import blueming from '../assets/blueming.jpg'
import nslcb from '../assets/nslcb.jpg'

export default {
    data(){
        return{
            favorite1: false,
            favorite2: false,
            favorite3: false,
            favorite4: false,
            favorite5: false,
            favorite6: false,
            favorite7: false,
            favorite8: false,
            favorite9: false,

            actual_color1: 'lightpink',
            actual_color2: 'lightpink',
            actual_color3: 'lightpink',
            actual_color4: 'lightpink',
            actual_color5: 'lightpink',
            actual_color6: 'lightpink',
            actual_color7: 'lightpink',
            actual_color8: 'lightpink',
            actual_color9: 'lightpink',

            lilac,
            celebrity,
            good_day,
            you_and_i,
            bbibbi,
            palette,
            eight,
            blueming,
            nslcb
        }
    },
    methods: {
        triggerFavorite1(){
            this.favorite1 = !this.favorite1
            if (this.favorite1){
                this.actual_color1 = 'plum'
            }
            else{
                this.actual_color1 = 'lightpink'
            }
        },
        triggerFavorite2(){
            this.favorite2 = !this.favorite2
            if (this.favorite2){
                this.actual_color2 = 'plum'
            }
            else{
                this.actual_color2 = 'lightpink'
            }
        },
        triggerFavorite3(){
            this.favorite3 = !this.favorite3
            if (this.favorite3){
                this.actual_color3 = 'plum'
            }
            else{
                this.actual_color3 = 'lightpink'
            }
        },
        triggerFavorite4(){
            this.favorite4 = !this.favorite4
            if (this.favorite4){
                this.actual_color4 = 'plum'
            }
            else{
                this.actual_color4 = 'lightpink'
            }
        },
        triggerFavorite5(){
            this.favorite5 = !this.favorite5
            if (this.favorite5){
                this.actual_color5 = 'plum'
            }
            else{
                this.actual_color5 = 'lightpink'
            }
        },
        triggerFavorite6(){
            this.favorite6 = !this.favorite6
            if (this.favorite6){
                this.actual_color6 = 'plum'
            }
            else{
                this.actual_color6 = 'lightpink'
            }
        },
        triggerFavorite7(){
            this.favorite7 = !this.favorite7
            if (this.favorite7){
                this.actual_color7 = 'plum'
            }
            else{
                this.actual_color7 = 'lightpink'
            }
        },
        triggerFavorite8(){
            this.favorite8 = !this.favorite8
            if (this.favorite8){
                this.actual_color8 = 'plum'
            }
            else{
                this.actual_color8 = 'lightpink'
            }
        },
        triggerFavorite9(){
            this.favorite9 = !this.favorite9
            if (this.favorite9){
                this.actual_color9 = 'plum'
            }
            else{
                this.actual_color9 = 'lightpink'
            }
        }
    }

}
</script>

<style>
    .song_sample{
        font-size: 50px;
        height: auto;
        width: 600px;
        border-radius: 20px;
        color: white;
        text-align: center;
        padding: 40px 0;
        margin: 40px auto;
    }
    img{
        width: 100px;
        height: 100px;
        display: block;
        margin-left: auto;
        margin-right: auto;
    }
</style>