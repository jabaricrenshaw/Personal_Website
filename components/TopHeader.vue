<template>
    <main>
        <div class="leftContent">
            <div class="d1">
                <nuxt-link id="name" to="/">
                    <p>Jabari<br>Crenshaw</p>
                </nuxt-link>
            </div>
        </div>
        <div class="rightContent">
            <div class="buttons">
                <nuxt-link to="/projects" class="rml"><p class="link">Projects</p></nuxt-link>
                <nuxt-link to="/about" class="rml"><p class="link">About</p></nuxt-link>
                <nuxt-link to="/resume" class="rml"><p class="link">Resume</p></nuxt-link>
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
    background: rgba(117,113,94,1);
}
.leftContent {
    width: 20%;
    height: 100%;
    display: flex;
    justify-content: flex-start;
    align-items: center;
}
.rightContent {
    width: 80%;
    height: 100%;
    display: flex;
    justify-content: flex-end;
    align-items: center;
}
.d1 {
    width: fit-content;
    margin: 0 15px;
}
#name {
    font-size: 2rem;
    color: black;
    text-decoration: none;
    filter: drop-shadow(0 0 3px black);
}
.buttons {
    display: flex;
    flex-direction: row;
    margin: 0 15px;
}
.link {
    color: black;
    text-decoration: none;
    font-size: 1.7rem;
    margin-left: 40px;
    line-height: 80px;
    border-radius: 10px;
}
.rml {
    text-decoration: none;
}
</style>
