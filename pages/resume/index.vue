<template>
    <main>
      <Header />
      <div class="content">
        <h2>Resume</h2>
      </div>
      <FileViewer />
    </main>
  </template>
  
  <script lang="ts" setup>
  import Header from '~/components/TopHeader.vue';
  import FileViewer from '~/components/FileViewer.vue';

  </script>
  
  <style lang="css" scoped>
  main{
    width: 100%;
  }
  .content {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
  }
  </style>