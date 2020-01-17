<template>
  <footer>
      <div id="logo">
          <img alt="logo" id="A" src="@/assets/img/logo.svg"/>
      </div>
      <div id="info">
        <div id="groupMembers">
          <h2>Group Members</h2>
          <p>Sabre Harrisson</p>
          <p>Sophie Quan</p>
          <p>Melissa Khan</p>
        </div>
        <div id="fontsSrc">
          <h2>Fonts Sources</h2>
          <p>Google Fonts</p>
          <p>Type Kits</p>
        </div>
        <div id="imgSrc">
          <h2>Image Sources</h2>
          <p>Sabre Harrisson</p>
        </div>
        <div id="audioSrc">
          <h2>Audio Sources</h2>
          <p>Melissa Khan</p>
        </div>
      </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style>

footer{
    width: 100%;
    height: auto;
    background-color: #EB9799;
    box-sizing: border-box;
    display: flex;
    flex-flow: row wrap;
    align-content: space-around;
    justify-content: center;
    align-content: center;
    justify-items: center;
}
footer p, footer h2{
    color: #fff;
    text-align: left
}
footer > div{
    margin: 10px 30px;
}
h2{
    font-size: 24px
}
#logo img{
    width: 100%;
    padding: 10px;
}
#logo > div{
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  width: 100%;
  height: auto;
}
#info{
    border-left: 2px solid #fff;
    display: flex;
    flex-flow: row;
    padding: 10px;
}
#info >div{
  margin: 20px;
}
</style>