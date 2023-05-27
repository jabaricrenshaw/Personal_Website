<template>
  <main>
    <Header />
    <div class="content">
      <h2>Home</h2>
    </div>
  </main>
</template>

<script lang="ts" setup>
import Header from '~/components/TopHeader.vue';

</script>

<style lang="css" scoped>
.content {
  height: calc(100vh - (80px + 15px + 3px + 20px));
  background-color: black;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  padding-top: 15px;
}
h2 {
  color: white;
}
</style>