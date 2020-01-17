<template>
    <header>
        <div id="headerContainer">
            <div id="headerimg">
                <img alt="HeaderSVG"  src="@/assets/img/logo.svg">
            </div>
            <img alt="HeaderSVG" id="headerLine" src="@/assets/img/bottomline.svg"/>
        </div>
    </header>
</template>

<script>
    export default{

    }
</script>

<style>
header {
    height: 30vh;
    width: 100%;
    background-color: #9ED2C9;
    flex-direction: row;
    justify-content: space-around;
}

#headerLine{
    position: relative;
    width: 100%;
    top: 15vh;
}
#headerimg{
    width: 100%;
    height: auto;
    position: absolute;
    z-index: 1;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: baseline;
    margin: 0 auto;
    top: 8vh;
}
img{
    width: 10%;
    
}
</style>