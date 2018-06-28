<template lang="html">
  <div id="game">

      <h1>Game!</h1>
      <hr>
      <p>
      Here is Game page!<br>
      </p>
      <gamepnl></gamepnl>

    </div>



</template>

<script>
import game_pnl from '../elements/gamepannel.vue';

export default {
  components:{
    'gamepnl':game_pnl
  },
  data(){
    return{
         }
  }
}
</script>

<style lang="css">

#game{
  padding: 10px 0px 10px;
  /* border: 1px dashed #BDBDBD; */
  height: auto;
  margin-left: auto;
  margin-right: auto;
  text-align: left;
  line-height: 2em;
}

</style>
