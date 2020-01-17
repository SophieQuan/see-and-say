<template>
  <div id="app">
    <Header/>
    <Description class="desc"/>
    <CardArea :data = "cardsInfo" :HistoryPick = "HistoryPick"/>
    <HistoryArea :HistoryPick = "HistoryPick"/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Description from './components/Description.vue'
import CardArea from './components/CardArea.vue'
import HistoryArea from './components/HistoryArea.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'app',
  components: {
    Header,
    Description,
    CardArea,
    HistoryArea,
    Footer
  },
  data(){
    return {
      cardsInfo:[
        {image:"card1.svg", audio:"A.mp3"},
        {image:"card2.svg", audio:"B.mp3"},
        {image:"card3.svg", audio:"C.mp3"},
        {image:"card4.svg", audio:"D.mp3"},
        {image:"card5.svg", audio:"E.mp3"},
        {image:"card6.svg", audio:"F.mp3"},
        {image:"card7.svg", audio:"G.mp3"},
        {image:"card8.svg", audio:"H.mp3"},
        {image:"card9.svg", audio:"I.mp3"},
        {image:"card10.svg", audio:"J.mp3"},
      ],
      HistoryPick: []
    }
  }
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #2c3e50;
  background-color: #f9f6e7;
  width: 100%;
  z-index: 15;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}

body {
  display: flex;
  justify-content: center;
  text-align: center;
  width: 100%;
  height: auto;
  margin:  0 auto;
}

.desc {
  text-align: center;
}
</style>
