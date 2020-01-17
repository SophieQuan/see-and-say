<template>
<div id = "historyArea">
    <img id="heading" alt="recently picked" src="@/assets/img/history_heading.svg"/>
    <HistoryCards v-for="(item, index) in HistoryPick" :key = "index" :image = "item"/>
</div>
</template>

<script>
import HistoryCards from '../components/HistoryCards.vue'
export default {
    name: "HistoryArea",
    components:{
        HistoryCards
    },
    props:{
        HistoryPick: Array
    }
}
</script>

<style>
    #historyArea{
        width: 60%;
        height: auto;
        border-radius: 20px;
        background-color: #9FD2C9;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-content: center;
        margin: 20px;
        justify-content: left;
        padding: 10px;
    }
    #heading{
        margin: auto 20px;
    }
</style>