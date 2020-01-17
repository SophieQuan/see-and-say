<template>
    <div id="cardArea">
        <cards v-for="(item, index) in data" :key = "index" :image = "item.image" :audio = "item.audio" :HistoryPick = "HistoryPick"/>    
    </div>
</template>

<script>
import cards from '../components/Cards.vue'

export default {
    name: "CardArea",
    components:{
        cards
    },
    props:{
        data: Array,
        HistoryPick: Array
    }
}
</script>

<style>
    #cardArea{
        width: 60%;
        height: auto;
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        justify-content: space-between;
    }

</style>