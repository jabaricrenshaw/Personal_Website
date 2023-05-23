<template>
    <main>
      <Header />
      <div class="content">
        <h2>Projects</h2>
      </div>
    </main>
  </template>
  
  <script lang="ts" setup>
  import Header from '~/components/TopHeader.vue';
  
  </script>
  
  <style lang="css" scoped>
  .content {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
  }
  </style>