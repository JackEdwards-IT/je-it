<template>
  <div class="portfolio">
    <b-container>
      <b-row>
        <div class="mx-auto">
          <h1>Portfolio</h1>
        </div>
      </b-row>

      <b-row class="form-group"></b-row>

      <!-- Card Scrabble game in C -->

      <b-card
        no-body
        class="overflow-hidden"
        style="max-width 400px;"
        text-variant="white"
      >
        <b-row no-gutters>
          <b-col md="5">
            <b-card-img
              :src="require('../assets/c-game.png')"
              alt="Screenshot of code initialising the game"
              class="rounded-0"
            ></b-card-img>
          </b-col>
          <b-col md="7">
            <b-card-body title="Word Game in C">
              <b-img
                src="https://img.shields.io/badge/-ANSI C-a8b9cc?logo=c&logoColor=white&style=plastic"
                height="23px"
                alt="ANSI C logo"
                class="mr-1"
              ></b-img>

              <b-card-text>
                This word game was developed within a C Programming software
                development subject. The assessment criteria for this project
                focused on memory management, dynamic data structures, file
                handling and adhering to the ANSI C language features.
              </b-card-text>
              <b-link
                target="_blank"
                href="https://github.com/JackEdwards-IT/c-scrabble"
                class="card-link"
                >Github</b-link
              >
              <b-link
                target="_blank"
                href="https://github.com/JackEdwards-IT/c-scrabble/raw/main/Project-Overview.pdf"
                class="card-link"
                >PDF Overview</b-link
              >
              <!-- <b-link target="_blank" href="#" class="card-link">PDF Overview</b-link> -->
            </b-card-body>
          </b-col>
        </b-row>
      </b-card>

      <b-row class="form-group"></b-row>

      <!-- Card Wordpress store  -->

      <b-card
        no-body
        class="overflow-hidden"
        style="max-width 400px;"
        text-variant="white"
      >
        <b-row no-gutters>
          <b-col md="5">
            <b-card-img
              :src="require('../assets/cat-site.png')"
              alt="Screenshot of the wordpress store page"
              class="rounded-0"
            ></b-card-img>
          </b-col>

          <b-col md="7">
            <b-card-body title="WordPress Store">
              <!-- Shield.io badges -->
              <b-img
                src="https://img.shields.io/badge/-PHP-777BB4?logo=php&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="PHP logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-HTML-E34F26?logo=html5&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="HTML logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-CSS-1572b6?logo=css3&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="CSS logo"
              ></b-img>

              <b-card-text>
                This WordPress Store was developed within my web-design minor.
                The project involved utilising WooCommerce and creating a custom
                theme for the site as well as a realistic plugin that a shop
                owner could utilise.
              </b-card-text>
              <b-link
                target="_blank"
                href="https://github.com/JackEdwards-IT/wordpress-petstore"
                class="card-link"
                >Github</b-link
              >
              <b-link
                target="_blank"
                href="http://pet-shop-demo.onlinewebshop.net/"
                class="card-link"
                >Live Demo</b-link
              >
              <b-link
                target="_blank"
                href="https://github.com/JackEdwards-IT/wordpress-petstore/raw/main/Project-Overview.pdf"
                class="card-link"
                >PDF Overview</b-link
              >
            </b-card-body>
          </b-col>
        </b-row>
      </b-card>

      <b-row class="form-group"></b-row>
      <!-- Card Portfolio website -->

      <b-card
        no-body
        class="overflow-hidden"
        style="max-width 400px;"
        text-variant="white"
      >
        <b-row no-gutters>
          <b-col md="5">
            <b-card-img
              :src="require('../assets/portfolio-site.png')"
              alt="Image of the portfolio site landing page"
              class="rounded-0"
            ></b-card-img>
          </b-col>
          <b-col md="7">
            <b-card-body title="Portfolio Website">
              <b-img
                src="https://img.shields.io/badge/-Vue.js-4fc08d?logo=vue.js&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="Vue.js logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-JS-f7df1e?logo=javascript&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="Javascript Logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-Bootstrap-7952b3?logo=bootstrap&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="Bootstrap Logo"
              ></b-img>

              <b-card-text>
                A simple static portfolio site (the one you are using now). This
                was my first project using Vue.js and Bootstrap.
              </b-card-text>
              <b-link
                target="_blank"
                href="https://github.com/JackEdwards-IT/je-it"
                class="card-link"
                >Github</b-link
              >
              <b-link
                target="_blank"
                href="https://trello.com/b/EPRlTF5B"
                class="card-link"
                >Trello</b-link
              >
              <!-- <b-link href="#" class="card-link">PDF Overview</b-link> -->
            </b-card-body>
          </b-col>
        </b-row>
      </b-card>
      <b-row class="form-group"></b-row>

      <!-- Card Crawler -->
      <!-- <b-card
        no-body
        class="overflow-hidden"
        style="max-width 400px;"
        text-variant="white"
      >
        <b-row no-gutters>
          <b-col md="5">
            <b-card-img
              :src="require('../assets/crawler.png')"
              alt="Screenshot of some javascript and jquery crawler code."
              class="rounded-0"
            ></b-card-img>
          </b-col>
          <b-col md="7">
            <b-card-body title="Web Scraper">
              <b-img
                src="https://img.shields.io/badge/-Vue.js-4fc08d?logo=vue.js&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="Vue.js Logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-Node.js-339933?logo=node.js&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="Node.js logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-PostgreSQL-336791?logo=postgresql&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="PostgreSQL logo"
              ></b-img>

              <b-card-text>
                <span style="font-size: 20px; color: yellow"
                  >Work In Progress</span
                >
                <br />
                For my capstone uni project I created a web crawler in Node.js
                as part of a small team. My job was to develop the backend for
                the crawler (REST API, Database and Crawler). I am currently in
                the process of creating the frontend for the application in
                Vue.js to replace the original Angular frontend created by
                another student.
              </b-card-text>
              <b-link
                target="_blank"
                href="https://github.com/JackEdwards-IT/web-crawler"
                class="card-link"
                >Github</b-link
              >
              <b-link
                target="_blank"
                href="https://trello.com/b/Rwrt0Uhr"
                class="card-link"
                >Trello</b-link
              > -->
      <!-- <b-link target="_blank" href="#" class="card-link">PDF Overview</b-link> -->
      <!-- 
            </b-card-body>
          </b-col>
        </b-row>
      </b-card> -->

      <!-- Card Portfolio website 2 -->

      <b-card
        no-body
        class="overflow-hidden"
        style="max-width 400px;"
        text-variant="white"
      >
        <b-row no-gutters>
          <b-col md="5">
            <b-card-img
              :src="require('../assets/terminal-portfolio.png')"
              alt="Image of the portfolio site landing page"
              class="rounded-0"
            ></b-card-img>
          </b-col>
          <b-col md="7">
            <b-card-body title="Terminal Style Website">
              <b-img
                src="https://img.shields.io/badge/-JS-f7df1e?logo=javascript&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="Javascript Logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-HTML-E34F26?logo=html5&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="HTML logo"
              ></b-img>
              <b-img
                src="https://img.shields.io/badge/-CSS-1572b6?logo=css3&logoColor=white&style=plastic"
                height="23px"
                class="mr-1"
                alt="CSS logo"
              ></b-img>

              <b-card-text>
                This is a small project utilising the Winbox.js library for the
                window manager and some custom Javascript for the basic terminal
                simulation. Type about or contact at the prompt to see the
                relevant windows.
              </b-card-text>
              <b-link
                target="_blank"
                href="https://github.com/JackEdwards-IT/terminal-style-portfolio"
                class="card-link"
                >Github</b-link
              >
              <b-link
                target="_blank"
                href="https://jackedwards-it.github.io/terminal-style-portfolio/"
                class="card-link"
                >Live Demo</b-link
              >
            </b-card-body>
          </b-col>
        </b-row>
      </b-card>
      <b-row class="form-group"></b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
/* Card titles */
h3 {
  font-family: "Titillium Web", sans-serif;
  color: white;
}
/* Card text */
p {
  font-family: "Titillium Web", sans-serif;
  color: white;
  letter-spacing: 1px;
}
/* Cart links */
a {
  color: white;
  text-decoration: underline !important;
}
/* Card custom border/bg*/
.card {
  background-color: #1d1d1d !important;
  border-color: rgba(161, 161, 161, 0.514) !important;
}
</style>
