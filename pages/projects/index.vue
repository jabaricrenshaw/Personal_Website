<template>
  <main>
    <Header />
    <div class="content">
      <h2 id="pageheader">Projects</h2>

      <div class="project-wrapper">
        <div class="project-main-header">
          <h3>Machine Learning</h3>
          <p>
            Each Machine Learning project was made for an AI/ML class and
            completed in Python. The ML Models were created using the Tensorflow
            libraries, and data cleaning was done using Pandas and Numpy.<br />See
            the code for each ML project
            <a
              class="external-link"
              href="https://github.com/jabaricrenshaw/Machine-Learning"
              target="_blank"
              >here</a
            >!
          </p>
        </div>
        <div class="wrapper-left">
          <div class="project-section project-section-left">
            <p class="project-section-header">Image Recognition</p>
            <p class="project-section-desc">
              Trained on the
              <a
                class="external-link"
                href="https://www.cs.toronto.edu/~kriz/cifar.html"
                target="_blank"
                >Cifar-10</a
              >
              dataset, the goal was to train a
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Convolutional_neural_network"
                target="_blank"
                >Convolutional Neural Network</a
              >
              that could correctly classify any one image from the dataset to one
              of ten textual descriptions.
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/blurry.png' />
          </div>
        </div>

        <div class="wrapper-right">
          <div class="project-section project-section-right">
            <p class="project-section-header">
              N-Queens Solver *(using
              <a
                class="external-link"
                href="https://deap.readthedocs.io/en/master/"
                target="_blank"
                >DEAP</a
              >
              Python library)
            </p>
            <p class="project-section-desc">
              The <i>N Queens</i> problem a.k.a
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Eight_queens_puzzle"
                target="_blank"
                >Eight Queens Puzzle</a
              >
              describes a challenge in placing N queens on an NxN chessboard such
              that no two queens can attack each other. The goal of this project
              was to build a
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Genetic_algorithm"
                target="_blank"
                >Genetic Algorithm</a
              >
              that will determine the placement of 8 neutral queens on an 8x8
              chessboard.
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/queens.png' />
          </div>
        </div>

        <div class="wrapper-left">
          <div class="project-section project-section-left">
            <p class="project-section-header">Network Intrusion Detection</p>
            <p class="project-section-desc">
              Trained on the 10% subset of the
              <a
                class="external-link"
                href="https://archive.ics.uci.edu/ml/datasets/kdd+cup+1999+data"
                target="_blank"
                >KDD ’99</a
              >
              dataset, the goal was to create a
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Convolutional_neural_network"
                target="_blank"
                >Fully Connected Neural Network</a
              >
              that best predicts the nature of a network connection and is able to
              categorize each a connection within two descriptions: decidedly
              "legitimate" and otherwise “untrustworthy”.
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/intrusion.png' style="transform: rotate(-30deg); max-height: 120px;" />
          </div>
        </div>

        <div class="wrapper-right">
          <div class="project-section project-section-right">
            <p class="project-section-header">Spam E-Mail Classifier</p>
            <p class="project-section-desc">
              Trained on the
              <a
                class="external-link"
                href="https://www.kaggle.com/datasets/neildavid/email-spam-classification-from-shantanu-dhakad"
                target="_blank"
                >Email Spam Classification</a
              >
              dataset found on Kaggle, this project features the use of a
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Convolutional_neural_network"
                target="_blank"
                >Convolutional Neural Network</a
              >
              and
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Recurrent_neural_network"
                target="_blank"
                >Recurrent Neural Network</a
              >
              . This project inteded to address the fact that the digital
              footprint of the average person grows with the side effect of
              greater online presence. This ML Model was trained on our dataset to
              be able to classify SPAM email using
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Text_segmentation#Word_segmentation"
                target="_blank"
                >tokenization</a
              >
              (in the form of word segmentation) and
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Tf%E2%80%93idf"
                target="_blank"
                >TF-IDF</a
              >
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/email.png' style="transform: rotate(-30deg); max-height: 150px;"/>
          </div>
        </div>

        <div class="wrapper-left">
          <div class="project-section project-section-left">
            <p class="project-section-header">Yelp Business Ratings</p>
            <p class="project-section-desc">
              Trained on the
              <a
                class="external-link"
                href="https://www.yelp.com/dataset"
                target="_blank"
                >Yelp Academic</a
              >
              dataset, the goal was to create a
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Natural_language_processing"
                target="_blank"
                >Natural Language Processor</a
              >
              that could estimate the rating of a business out of 5 stars based on
              language used in the written reviews of that business. Language
              evaluation was done using
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Tf%E2%80%93idf"
                target="_blank"
                >TF-IDF</a
              >
              statistics. These statistics derived from the words in business
              reviews essentially had the power to increase or reduce the star
              rating of a business if the language used was deemed to be
              "positive" or "negative" reinforcement reflecting customer
              experience.
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/star.png' />
          </div>
        </div>

        <div class="project-main-header">
          <h3>Games / Graphics</h3>
          <p class="project-section-desc"></p>
        </div>
        <div class="wrapper-left">
          <div class="project-section project-section-left">
            <p class="project-section-header">Mandelbrot Set</p>
            <p class="project-section-desc">
              Made using the
              <a
                class="external-link"
                href="https://www.raylib.com/"
                target="_blank"
                >Raylib</a
              >
              development library in C++. The idea came from browsing the web
              and finding interesting math equations that could be be plotted 
              in 2D/3D space to create a 
              <a
                class="external-link"
                href="https://en.wikipedia.org/wiki/Fractal"
                target="_blank"
                >fractal</a
              >.
              I wanted to complete this project to get better at graphics development
              and working with arrays >= 2 dimensions. Other than that, it was fun and 
              just looks cool to me! The simulation is availalbe for free on GitHub 
              <a
                class="external-link"
                href="https://github.com/jabaricrenshaw/mandelbrot-set"
                target="_blank"
                >here</a
              >! View the README to get started.
            </p>
          </div>
          <div class="project-section-image-left">
            <img src='images/mandelbrot.png' />
          </div>
        </div>

        <div class="wrapper-right">
          <div class="project-section project-section-right">
            <p class="project-section-header">Flappy Fish</p>
            <p class="project-section-desc">
              Made using the
              <a
                class="external-link"
                href="https://www.pygame.org/news"
                target="_blank"
                >PyGame</a
              >
              library for Python, it started off as an ambitious project to learn
              Python. The idea to recreate <i>"Flappy Fish"</i> was sort of
              un-original, but I figured if I could manage to complete this game
              my goal would be achieved. The game is availalbe for free. Clone the
              repo and play Flappy Fish
              <a
                class="external-link"
                href="https://github.com/jabaricrenshaw/Flappy-Fish"
                target="_blank"
                >here</a
              >!
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/fish.png' style="transform: rotate(-30deg); max-height: 60px;" />
          </div>
        </div>

        <div class="wrapper-left">
          <div class="project-section project-section-left">
            <p class="project-section-header">Spider "Walk-It" Game</p>
            <p class="project-section-desc">
              Made using the
              <a
                class="external-link"
                href="https://www.codenameone.com/"
                target="_blank"
                >CodenameOne</a
              >
              framework for Java as a semester long class project. As being the
              successor game-based project to Flappy Fish, this project was made
              with certain design patterns in mind: Singleton for the "Player",
              Iterator for game objects with the same types. Including abstract
              classes, inheritance, and interfaces (All sorts of Java specific
              terms but translates to other OOP languages). The game is availalbe
              for free. Clone the repo and play "Walk-It"
              <a
                class="external-link"
                href="https://github.com/jabaricrenshaw/Spider-Game"
                target="_blank"
                >here</a
              >! View the README to get started.
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/spider.gif' style="max-height: 100px;" />
          </div>
        </div>

        <div class="project-main-header">
          <h3>Larger Projects</h3>
          <p class="project-section-desc">
            *Projects that deserve a seperate category.
          </p>
        </div>
        <div class="wrapper-left">
          <div class="project-section project-section-left">
            <p class="project-section-header">MITLL Racecar</p>
            <p class="project-section-desc">
              As part of a project of employment, I built a self-driving rc car meant to follow lines,
              navigate paths between walls, and respond with movement based on stimuli (i.e. QR code).
              The original project was created by the MIT Lincoln Laboratory
              Read more about this experience on my
              <a
                class="external-link"
                href="/resume"
                target="_blank"
                >resume</a
              >!
              Build your own self-driving rc car following this
              <a
                class="external-link"
                href="https://mitll-racecar-mn.readthedocs.io/en/latest/"
                target="_blank"
                >guide</a
              >!
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/rc.jpg' />
          </div>
        </div>

        <div class="wrapper-right">
          <div class="project-section project-section-right">
            <p class="project-section-header">Peoplesense Dashboard</p>
            <p class="project-section-desc">
              This project was completed as a capstone project with a group total
              of 8 members. The dashboard application is a web-based product which
              displays the current or historical occupancy counts of Amtrak trains
              in N. California. The dashboard fully customizable using widgets and
              users are tracked by Amtrak agencies via login authentication. This
              project was a complete overhaul of our client's existing solution
              and involved web development, database management, and project
              deployment for public use. Since the project was accepted by our client,
              the current owner of the codebase is
              <a
                class="external-link"
                href="http://www.glocol.net/"
                target="_blank"
                >Glocol Networks</a
              >.
            </p>
          </div>
          <div class="project-section-image-right">
            <img src='images/dashboard.png' />
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script lang="ts" setup>
import Header from '~/components/TopHeader.vue'

</script>

<style lang="css" scoped>
.content {
  background-color: #212121;
  width: 100%;
  padding-top: 10px;
  color: white;
}
#pageheader {
  text-align: center;
  color: white;
}
.wrapper-left{
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
}
.wrapper-right{
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
}
.project-wrapper {
  display: flex;
  flex-direction: column;
  padding: 0 3%;
  margin: auto;
  max-width: 1050px;
}
.project-section {
  width: 60%;
  padding-bottom: 10px;
}
.project-section-image-left img{
  max-height: 170px;
}
.project-section-image-right img{
  max-height: 170px;
}
.project-section-desc {
  padding-top: 2px;
}
.external-link {
  text-decoration: none;
  color: orange;
  font-style: italic;
}
.project-main-header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  margin: auto;
  width: 85%;
  padding-bottom: 10px;
  padding-top: 20px;
}
.project-section-header {
  font-weight: bold;
  border-bottom: 1px solid white;
  padding-bottom: 2px;
  font-style: italic;
}
.project-section-left {
  padding-right: 10px;
}
.project-section-right {
  padding-left: 10px;
}
</style>
