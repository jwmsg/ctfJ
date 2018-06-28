<template>

  <div id="app">
    <headers></headers>
    <bodys></bodys>
    <footers></footers>

  </div>

</template>

<script>
import header from './components/Header.vue';
import myBody from './components/MyBody.vue';
import footer from './components/Footer.vue';

export default {
  name:"app",
  components:{
    'headers': header,
    'bodys' : myBody,
    'footers' : footer
  }
}
</script>

<style>
#app {

}
p{
  width: 100%;
  padding: 20px 0px 0px;
  line-height: 1.6em;
  color: #5d5d5d;
  margin-left: auto;
  margin-right: auto;
}
h1{

  padding: 0px 0px 20px;
  margin-left: auto;
  margin-right: auto;
  left: inherit;
  right: inherit;
}
hr{
  margin-left: auto;
  margin-right: auto;
  left: inherit;
  right: inherit;
}
*{
    margin:0;
    padding:0;
}

body{
    font:15px/1.3 'Open Sans', sans-serif;
    color: #5e5b64;
    text-align:center;
}

a, a:visited {
    outline:none;
    color:#5e5b64;
    text-decoration:none
}

a:hover{
    text-decoration:none;
}

section, footer, header, aside, nav{
    display: block;
}
pre{
  color: #000000;
}

</style>
