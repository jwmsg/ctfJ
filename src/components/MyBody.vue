<template lang="html">
  <div id="body">
    <bodys></bodys>
  </div>
</template>

<script>
import home from './Menus/home.vue';
import WErr from './Menus/Error.vue';
import Winfo from './Menus/infomation.vue';
import Wscore from './Menus/score.vue';
import Wgame from './Menus/game.vue';

let locations = (window.location.pathname).replace('/','');
  if(locations === '')
    locations = 'home';

let pages = home;

  switch (locations) {
    case 'home':
          pages = home;
      break;

    case 'infomation':
          pages = Winfo;
      break;

    case 'score':
          pages = Wscore;
      break;

    case 'game':
          pages = Wgame;
    break;

    default:
          pages = WErr;

  }

export default {
  components:{
    'bodys': pages
  },
  data(){

    return
    {

    }
  }
}
</script>

<style lang="css">
#body{
  height:100%;
  width: 60%;
  margin-left: auto;
  margin-right: auto;
}
</style>
