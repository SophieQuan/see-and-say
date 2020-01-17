<template>
    <div id="historyCards">
        <img :src="require(`../assets/img/${image}`)" alt="abc learning app"/>
    </div>
</template>

<script>
export default {
    name: "HistoryCards",
    props:{
        image: String
    }
}
</script>

<style>
    #historyCards{
        width: 15%;
        height: auto;
        margin: auto
    }
    img{
        width: 10%;
    }
    #historyCards img{
        width: 100%;
        height: auto;
        object-fit: cover;
    }

</style>