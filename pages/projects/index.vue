<template>
  <main>
    <Header />
    <div class="content">
      <h2 id="pageheader">Projects</h2>
      
      <div class="project-wrapper">

        <div v-for="project in projects">
          <div class="project-main-header">
            <h3>{{ project.Subject }}</h3>
            <span v-html="project.Description" />
          </div>
          <div :class="[leftAlign ? 'wrapper-left' : 'wrapper-right', 'wrapper']" v-for="item in project.Projects">
            <div :class="[leftAlign ? 'project-section-left' : 'project-section-right', 'project-section']">
              <p class="project-section-header">{{ item.Name }}</p>
              <p class="project-section-desc">
                <span v-html="item.Description" />
              </p>
            </div>
            <div class="project-section-image">
              <img :src="item.Image" class="project-section-image">
            </div>
            {{ swapAlign() }}
          </div>
          <span v-if="!leftAlign">{{ swapAlign() }}</span>
        </div>

      </div>
    </div>
  </main>
</template>

<script lang="ts" setup>
import Header from '~/components/TopHeader.vue'
import { onMounted, ref } from 'vue'

const leftAlign = ref()

onMounted(() => {
  leftAlign.value = ref(true)
})

const swapAlign = () => {
  leftAlign.value = !leftAlign.value
}

const projects = [
  {
    Subject: "Machine Learning",
    Description: String.raw`
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
          `,
    Projects: [
      {
        Name: "Image Recognition",
        Description: String.raw`
          <p>
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
        `,
        Image: "images/blurry.png"
      },
      {
        Name: "N-Queens Solver",
        Description: String.raw`
          <p>
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
            using
            <a
              class="external-link"
              href="https://deap.readthedocs.io/en/master/"
              target="_blank"
              >DEAP</a
            >
            that will determine the placement of 8 neutral queens on an 8x8
            chessboard.
          </p>
        `,
        Image: "images/queens.png"
      },
      {
        Name: "Network Intrusion Detection",
        Description: String.raw`
          <p>
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
        `,
        Image: "images/intrusion.png"
      },
      {
        Name: "Spam E-Mail Classifier",
        Description: String.raw`
          <p>
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
        `,
        Image: "images/email.png"
      },
      {
        Name: "Yelp Business Ratings",
        Description: String.raw`
          <p>
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
        `,
        Image: "images/star.png"
      }
    ]
  },
  {
    Subject: "Games / Graphics",
    Description: "",
    Projects: [{
        Name: "Mandelbrot Set",
        Description: String.raw`
          <p>
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
        `,
        Image: "images/mandelbrot.png"
      },
      {
        Name: "Physics Simulation",
        Description: String.raw`
          <p>
            Once again, this project was made using 
            <a
              class="external-link"
              href="https://www.raylib.com/"
              target="_blank"
              >Raylib</a
            >
            in C++. I wanted to apply the concepts of kinematics, gravity,
            and force based physics in a "real-time" environment where the
            code is as period correct as possible. I would hope that
            if this project is written well enough going forward, that
            I could begin to support others to fork this project as a good base
            for their own physics visualization ideas.
            <a
              class="external-link"
              href="https://github.com/jabaricrenshaw/Physics_Sim"
              target="_blank"
              >here</a
            >! View the README to get started.
          </p>
        `,
        Image: "images/fsx.gif"
      },
      {
        Name: "Flappy Fish",
        Description: String.raw`
          <p>
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
        `,
        Image: "images/fish.png"
      },
      {
        Name: "Spider \"Walk-It\" Game",
        Description: String.raw`
          <p>
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
        `,
        Image: "images/spider.gif"
      }]
  },
  {
    Subject: "Larger Projects",
    Description: "*Projects that deserve a seperate category.",
    Projects: [{
      Name: "MITLL Racecar",
      Description: String.raw`
        <p>
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
      `,
      Image: "images/rc.jpg"
    },
    {
      Name: "Peoplesense Dashboard",
      Description: String.raw`
        <p>
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
      `,
      Image: "images/dashboard.png"
    }]
  }
]

</script>

<style>
.external-link {
  text-decoration: none;
  color: orange;
  font-style: italic;
}
</style>

<style lang="css" scoped>
main {
  height: 100vh;
}
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
.wrapper{
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  padding-bottom: 50px;
}
.wrapper-left{
  flex-direction: row;
}
.wrapper-right{
  flex-direction: row-reverse;
}
.project-wrapper {
  display: flex;
  flex-direction: column;
  padding: 0 3%;
  margin: auto;
  max-width: 1050px;
}
.project-section {
  text-align: left;
  width: 60%;
}
.project-section-image img {
  max-height: 170px;
}
.project-section-desc {
  padding-top: 2px;
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
  padding-right: 25px;
}
.project-section-right {
  padding-left: 25px;
}
</style>
