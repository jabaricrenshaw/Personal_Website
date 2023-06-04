<template>
    <main>
        <div class="leftContent">
            <div class="d1">
                <NuxtLink id="name" to="/">Jabari<br>Crenshaw</NuxtLink>
            </div>
        </div>
        <div class="centerContent">
            
        </div>
        <div class="rightContent">
            <div class="buttons">
                <NuxtLink to="/projects" class="link">Projects</NuxtLink>
                <NuxtLink to="/resume" class="link">Resume</NuxtLink>
            </div>
        </div>
    </main>   
</template>

<script lang="ts" setup>

</script>

<style lang="css" scoped>
main{
    width: 100%;
    height: 80px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    background-color: #141414;
    border-bottom: white 4px solid;
    padding-bottom: 10px;
    padding-top: 10px;
}
.leftContent {
    width: 16%;
    height: 100%;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    margin-left: 20px;
}
.d1 {
    width: fit-content;
}
#name {
    font-size: 2rem;
    color: #a0a0a0;
    text-decoration: none;
    
    transition: 0.3s;
}
#name:hover{
    color: white;
    filter: drop-shadow(0 0 5px white);
}
.centerContent{
    width: 49%;
}
.rightContent {
    width: 35%;
    display: flex;
    align-items: center;
    margin-right: 20px;
}
.buttons{
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
}
.link{
    color:#a0a0a0;
    font-size: 1.4rem;
    text-decoration: none;

    position: relative;
    letter-spacing: 0.5px;
    padding: 0 0;
    transition: 0.3s;
}
.link:after{
    content: "";
    position: absolute;
    background-color: orange;
    height: 3px;
    width: 0;
    left: 0;
    bottom: -0.2rem;
    transition: 0.3s;
}
.link:hover{
    color: white;
}
.link:hover:after{
    width: 100%;

}
</style>
