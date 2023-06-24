<template>
  <main>
    <Header />
    <div class="content">
      <h2 id="pageheader">Home</h2>
      <div class="home-wrapper">

        

        <div class="section-one add-bottom-pad">
          <div class='profile-img'>
            <img  src='images/profileimage.jpg'/>
          </div>
          <div class="section-one-one">
            <div class="text-area add-bottom-pad">
              <span style="font-weight: bold;">
                Welcome to my personal website and development log!
              </span>
              <br />
              I'm ecstatic to have you here. As you navigate through this site,
              I hope you'll discover my passion for software development or maybe
              give you some inspiration to create something new of your own.
              <br />
              You'll also get a chance to know a little more about me if you're
              curious and came from my LinkedIn.
            </div>

            <div class="text-area">
              <span style="font-weight: bold;">
                What else should you expect to see? 
              </span>
              <br />
              Everything here is to acknowledge and document some of my personal
              feats as a developer. The Projects page will only continue to grow
              every month to reflect whatever topic I may be focused on at the moment.
            </div>
          </div>
        </div>

        <div class="section-two">
          <div class="text-area add-bottom-pad">
            <span style="font-weight: bold;">
              Allow me to introduce myself! 
            </span>
            <br />
            I'm currently an amateur software developer and recent
            graduate of Sacramento State (Stingers up!).
            <br />
            In terms of software development, my areas of expertise are
            full stack development, cloud computing, and machine learning. The
            projects page is intended to highlight the skills I have used on
            my projects.
          </div>
          <div class="text-area">
            Beyond my hard work behind the desk, I find solace and excitement
            in a few hobbies that I keep up with. I could be soaring through
            the streets on my skateboard, exploring the serene waters of the Folsom
            lake while kayaking, or having a light gaming session.
          </div>
        </div>
      </div>     
    </div>
  </main>
</template>

<script lang="ts" setup>
import Header from '~/components/TopHeader.vue';

</script>

<style lang="css" scoped>
main {
  height: 100vh;
}
.content {
  background-color: #212121;
  width: 100%;
  padding-top: 10px;
  color: white;
  /*display: flex;
  flex-direction: column;*/
}
.profile-img {
  height: 300px;
  padding: 0 20px 0 0;
}
.profile-img img {
  width: 300px;
  height: 300px;
  border-radius: 150px;
  box-shadow: rgb(63, 63, 63) 0 0 8px 8px;
}

#pageheader {
  text-align: center;
  color: white;
}
.home-wrapper {
  padding: 20px 15% 0 15%;
  margin: auto;
  max-width: 1050px;
}
.section-one{
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.section-one-one{
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.section-two{
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.text-area {
  
}
.add-bottom-pad {
  padding: 0 0 30px 0;
}
</style>