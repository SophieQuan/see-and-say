<template>
    <div class="description">
        <div id="texty">
            <h2>Welcome to the fun world of ABC!</h2>
            <p>ABC is a fun learning module for kids. Let’s learn the alphabet together. <strong >Click on a card</strong> to get started for a wonderful suprise!</p>
        </div>
    </div>
</template>

<script>
   export default{
   }
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Open+Sans&display=swap');
@import url("https://use.typekit.net/spp7yjs.css");

.description {
    background-image: url("../assets/img/desc.svg");
    background-repeat: no-repeat;
    width: 100%;
    height: 400px;
    background-position: center;
}

#texty {
    padding: 15vh 2vw 0 2vw;
    width: 60%;
    margin: 0 auto;
}

h2 {
    font-family: brandon-grotesque, sans-serif;
    font-weight: 700;
    font-style: normal;
    color: #05ab94;
    font-size: 36px;
    
}

p {
    font-family: "Open Sans", sans-serif;
    color: #05ab94;
    font-size: 18px;
}
strong{
    color: #EB9699
}
</style>