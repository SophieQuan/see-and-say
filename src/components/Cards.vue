<template>
    <div id="card" @click="playAudio(require(`../assets/audio/${audio}`)), playBackground(require(`../assets/audio/musicBackground.mp3`)), addRecentlyPick()">
        <img :src="require(`../assets/img/${image}`)" alt="abc learning app"/>
    </div>
</template>

<script>
   export default{
        name: "cards",
        props: {
            image: String,
            audio: String,
            HistoryPick: Array
        },
        methods: {
            playBackground(theFile){
                let backgroundSound = new Audio(theFile);
                backgroundSound.volume = 0.05;
                backgroundSound.play();
            },
            playAudio(audioPath){
                let myaudio = new Audio(audioPath);
                myaudio.volume = 1;
                myaudio.play();
            },
            addRecentlyPick(){
                if(this.HistoryPick.length >=10){
                    this.HistoryPick.shift();
                }
                this.HistoryPick.push(this.image);
            },
        },
        
    }
</script>

<style scoped>
#card {
    width: 20%;
    height: auto;
    display: flex;
    flex-direction: column;
}

#card img {
    padding: 10px;
    text-align: center;
    width: 100%;
}
#card img:hover{
    box-shadow: inset 0 0 0 70px #EFEAD5;
    border-radius: 20px;
    transform: scale(1.05);
    transition: ease-in-out;
    
}

</style>