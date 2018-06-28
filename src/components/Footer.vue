<template lang="html">
  <div id = "footer">
    <div id="footerbox">
      <div id="loginbox">
          Username <br><input type="text" class="INP_Login_Id">
          Password <br><input type="password" class="INP_Login_Pw">
          <br>
          <br>
          <button type="button" id = "BTN_Login" class="BTN_Login">Login</button>
      </div>


    </div>
    <hr>
    <a href="https://jwmsg.kr" class="jwlink"> Made by Jaewan Jeong</a>
  </div>
</template>

<script>
export default {
  data () {
    return {


    }
  }
}
</script>

<style lang="css">

#footer{
  padding: 10px 0px 10px;

  height: auto;
  width:100%;

  position:absolute;
  bottom:0px;
  left: inherit;
  right: inherit;
  left:50%;
  transform:translateX(-50%);
  background: #0d54a6;
}
#footerbox{
  margin-right: auto;
  margin-left: auto;
  width:60%;
  height: 200px;
  /* border: 1px dashed #BDBDBD; */
  text-align: left;
  color: #FFFFFF;

}
#loginbox{
  line-height: 2em;
  width:20%;
  height: 200px;
  font-style: bold;
  /* border: 1px dashed #BDBDBD; */

}
a.jwlink{
  font-size: 18px;
  color: #FFFFFF;
}
button.BTN_Login{
  width: 40%;
  padding: 10px 5px 10px;
  background: #00FFBF;
  border-radius: 5px;
  border: 1;
  outline: 0;
  float: right;
}
p.loginfrm{
  color: #FFFFFF;
}
input.INP_Login_Id, input.INP_Login_Pw{
  width: 100%;
  height: 30px;
  border-radius: 5px;
  border: 0;
  outline: 0;
  font-size: 20px;
  right: 0px;
}
</style>
