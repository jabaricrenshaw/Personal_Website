<template>
  <main>
    <Header />
    <div class="content">
      <h2 id="pageheader">Projects</h2>

      <div class="projects">
        <h3 class="project-header">Machine Learning</h3>
        <p>
          Each Machine Learning project was completed in Python. The ML Models
          were created using the Tensorflow libraries, data cleaning was done
          using Pandas and Numpy.
        </p> 
        
        <div class="project-section project-section-left">
          <p class="project-section-header">Image Recognition</p>
          <p>
            My Image Recognition Model was trained on the <a href="https://www.cs.toronto.edu/~kriz/cifar.html" target="_blank">"Cifar-10"</a>
            dataset. The goal was to train an ML Model that could correctly any one image
            from the dataset to one of ten textual descriptions. 

          </p>
        </div>
          
        <div class="project-section project-section-right">
          <p class="project-section-header">N-Queens</p>
          <p>
            My Image Recognition Model was trained on the <a href="https://www.cs.toronto.edu/~kriz/cifar.html" target="_blank">"Cifar-10"</a>
            dataset. The goal was to train an ML Model that could correctly any one image
            from the dataset to one of ten textual descriptions. 

          </p>
        </div>

        <div class="project-section-left">
          <p class="project-section-header">Network Intrustion</p>
        </div>

        <div class="project-section-right">
          <p class="project-section-header">Spam E-mail Classifier</p>
        </div>
        
        <div class="project-section-left">
          <p class="project-section-header">Yelp Ratings</p>
        </div>
        


        <h3 class="project-header">Games</h3>
        <div class="project-section project-section-right">
          <p class="project-section-header">Flappy Fish</p>

          <p class="project-section-header">Spider "Walk-It" Game</p>

        </div>

        <h3 class="project-header">Larger Projects and Tools</h3>
        <div class="project-section project-section-left">
          <p class="project-section-header">PeopleSense Dashboard</p>

          <p class="project-section-header">Autonomous Racing Vehicle (MITLLRacecar)</p>

          <p class="project-section-header">Client/Server Messaging Platform</p>

          <p class="project-section-header">GitOscar</p>

        </div>
      </div>

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
  padding-top: 15px;
  color: white;
}
#pageheader {
  text-align: center;
  color: white;
}
.projects{
  margin: 20px 3% 0 3%;
  background-color: yellow;
  display: flex;
  flex-direction: column;
}
.project-header{
  border-bottom: 1px solid white;
}
.project-section{
  margin: 10px 0 40px 0;
  width: 60%;
  display: flex;
  flex-direction: column;
}
.project-section-left{
  text-align: left;
  background-color: red;
  display: flex;
}
.project-section-right{
  background-color: green;
  justify-content: flex-end;
}
.project-section-header{
  margin: 10px 0 0 0;
}
</style>