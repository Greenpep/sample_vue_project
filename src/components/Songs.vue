<template>
  <div class="songs">
      <div class="song_sample" @click="triggerFavorite1" v-bind:style=" {'background-color': actual_color1} ">
          <img :src="`../assets/LILAC.jpeg`" :alt="lilac_img">
          LILAC
      </div>
      <div class="song_sample" @click="triggerFavorite2" v-bind:style=" {'background-color': actual_color2}">
          Celebrity
      </div>
      <div class="song_sample" @click="triggerFavorite3" v-bind:style=" {'background-color': actual_color3}">
          Good Day
      </div>
      <div class="song_sample" @click="triggerFavorite4" v-bind:style=" {'background-color': actual_color4}">
          You And I
      </div>
      <div class="song_sample" @click="triggerFavorite5" v-bind:style=" {'background-color': actual_color5}">
          BBIBBI
      </div>
      <div class="song_sample" @click="triggerFavorite6" v-bind:style=" {'background-color': actual_color6}">
          Palette
      </div>
      <div class="song_sample" @click="triggerFavorite7" v-bind:style=" {'background-color': actual_color7}">
          eight
      </div>
      <div class="song_sample" @click="triggerFavorite8" v-bind:style=" {'background-color': actual_color8}">
          Blueming
      </div>
      <div class="song_sample" @click="triggerFavorite9" v-bind:style=" {'background-color': actual_color9}">
          Not Spring, Love, or Cherryblossom
      </div>
  </div>
</template>

<script>
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
</style>