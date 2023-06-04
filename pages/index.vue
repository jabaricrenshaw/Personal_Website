<template>
  <main>
    <Header />
    <div class="content">
      <h2 id="pageheader">Home</h2>
      <div class="home-wrapper">
        <p>This is me.</p>
      </div>
    </div>
  </main>
</template>

<script lang="ts" setup>
import Header from '~/components/TopHeader.vue';

</script>

<style lang="css" scoped>
.content {
  background-color: #212121;
  width: 100%;
  height: calc(100vh - (80px + 13px + 20px));
  padding-top: 10px;
  color: white;
}
#pageheader {
  text-align: center;
  color: white;
}
.home-wrapper {
  display: flex;
  flex-direction: column;
  padding: 0 3%;
  margin: auto;
  max-width: 1050px;
}
</style>