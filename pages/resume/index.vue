<template>
  <main>
    <Header />
    <div class="content">
      <h2 id="pageheader">Resume</h2>
      <FileViewer />
    </div>
  </main>
</template>
  
<script lang="ts" setup>
import Header from '~/components/TopHeader.vue';
import FileViewer from '~/components/FileViewer.vue';

</script>
  
<style lang="css" scoped>
h2 {
  color: white;
}
.content {
  width: 100%;
  text-align: center;
  height: calc(100vh - (80px + 15px + 3px + 20px));
  padding-top: 15px;
  background-color: #212121;
}
#pageheader{
  margin-top: -5px;
  padding-bottom: 20px;
}
</style>