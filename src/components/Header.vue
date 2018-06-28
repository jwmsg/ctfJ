<template lang="html">
      <div>
        <br>
        <a href = "/">
          <img src="../assets/J_Logo.jpg" height="100px">
          <h1>CTF-J</h1>
        </a>
      <br>
      <nav v-bind:class="active" v-on:click.prevent>
        <a href="/" class="home" v-on:click="makeActive('home')">Main</a>
        <a href="/infomation" class="infomation" v-on:click="makeActive('infomation')">Infomation</a>
        <a href="/score" class="score" v-on:click="makeActive('score')">ScoreBoard</a>
        <a href="/game" class="game" v-on:click="makeActive('game')">Game</a>
      </nav>
    </div>


</template>

<script>
let locations = (window.location.pathname).replace('/','');
  if(locations === '')
    locations = 'home';
export default {

      data () {
        return {
          active: locations

        }
      },
      methods: {
        makeActive: function(item){
            this.active = item;
            window.location.href=item;
        }
    }
}
</script>

<style lang="css">


/*-------------------------
    The menu
--------------------------*/

nav{
    width: 100%;
    display:inline-block;
    margin:20px auto 45px;
    background-color:#0d54a6;
    box-shadow:0 1px 1px #ccc;
    border-radius:2px;
}

nav a{

    display:inline-block;
    padding: 18px 100px;
    color:#fff !important;
    font-weight:bold;
    font-size:18px;
    text-decoration:none !important;
    line-height:1;
    text-transform: uppercase;
    background-color:transparent;

    -webkit-transition:background-color 0.25s;
    -moz-transition:background-color 0.25s;
    transition:background-color 0.25s;
}

nav a:first-child{
    border-radius:2px 0 0 2px;
}

nav a:last-child{
    border-radius:0 2px 2px 0;
}

nav.home .home,
nav.infomation .infomation,
nav.score .score,
nav.game .game,
nav.account .account{
    background-color:#8e60a6;
}

</style>
