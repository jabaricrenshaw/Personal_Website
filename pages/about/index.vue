<template>
  <main>
    <Header />
    <div class="content">
      <h2>About</h2>
    </div>
    I am a doo doo head
  </main>
</template>

<script lang="ts" setup>
import Header from '~/components/TopHeader.vue';

</script>

<style lang="css" scoped>
h2 {
  color: white;
}
.content {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
}
</style>