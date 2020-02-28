<template>
    <div class="logos-wrapper">
        <h2 class="title-header">Logos</h2>
        <div class="item-logos">
            <img class="logo" alt="Vue logo" src="../assets/applelogo.png">
        </div>
        <div class="item-logos">
            <img class="logo" alt="Vue logo" src="../assets/avengerlogo.png">
        </div>
        <div class="item-logos">
            <img class="logo" alt="Vue logo" src="../assets/instagramlogo.png">
        </div>
        <div class="item-logos">
            <img class="logo" alt="Vue logo" src="../assets/applelogo.png">
        </div>
        <div class="item-logos">
            <img class="logo" alt="Vue logo" src="../assets/avengerlogo.png">
        </div>
        <div class="item-logos">
            <img class="logo" alt="Vue logo" src="../assets/instagramlogo.png">
        </div>
    </div>
</template>

<script>
    export default {
        name:"Logos",
    }
</script>

<style scoped>
.title-header{
    margin-bottom: 40px;
    text-align:left;
}
.logos-wrapper {
    width: 60%;
    overflow: hidden;
    margin: auto;
    
}

.item-logos{
    float: left;
    margin-right: 70px;
    margin-bottom: 70px;
    width:  150px;
    height: 150px;
    
}

.logo{
    width:150px;
    height: 150px;
}
</style>