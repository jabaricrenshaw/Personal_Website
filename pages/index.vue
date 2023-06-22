<template>
  <main>
    <Header />
    <div class="content">
      <h2 id="pageheader">Home</h2>
      <div class="home-wrapper">

        <div class='profile-img'>
          <img  src='images/profileimage.jpg'/>
        </div>
            -----Opening-----<br />
            Welcome to my personal website and development log! I'm ecstatic
            to have eyes on it. As you navigate through this site, I hope
            you'll discover my passion for software development or maybe give
            you some inspiration to create something new.
            <br />----------------------
        </div>
        <div>
            ----------Introduction------------<br />
            Allow me to introduce myself and give you a glimpse into who I am

            I'm Jabari, currently an amateur software developer and recent
            graduate of Sacramento State (Stingers up!).

            In terms of software development, my areas of expertise are
            full stack development, cloud computing, and machine learning.
            
            This site is here to acknowledge some of my personal feats as a
            developer and the Projects page will only continue to grow from here
            every month.

            Beyond my hard work behind the desk, I find solace and excitement
            in a few thrilling hobbies. Whetther it's soaring through the streets
            on my skateboard, exploring the serence waters of the Folsom lake while
            kayaking, or immersing myself in my favorite rotation of video games.
            <br />------------------------
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
.profile-img {
  float: left;
  padding: 0 15px 15px 0;
}
.profile-img img {
  width: 320px;
  border-radius: 160px;
}

#pageheader {
  text-align: center;
  color: white;
}
.home-wrapper {
  padding: 0 3%;
  margin: auto;
  max-width: 1050px;
}
</style>