<template>
  <div id="app">
    <imageHeader></imageHeader>
    <main>
      <div class="row">
        <div class="col-md-12">
          <div class="body-container">
            <h2 class="display-4">FACULTIES</h2>
            <p class="lead">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </p>
            <div v-for="object in objects" :key="object.Teaching">
            <div class="instructor-container">
              <div class="card-instructor">
                <div class="c1">
                  <img
                    class="personimg"
                    :src="object.image"
                    alt="Avatar"
                  />
                  <div><p>{{object.name}}</p></div>
                  <div><p class="titlename">{{object.titlename}}</p></div>
                </div>
                <div class="c2">
                  <div class="card-text-box">
                    <p class="cardp">
                      <b>Title: </b> {{object.title}}
                    </p>
                    <p class="cardp"><b>Experience</b>: {{object.Experience}}</p>

                    <p class="cardp">
                      <b>Bio:</b> {{object.Bio}}
                    </p>
                    <p class="cardp"><b>Email:</b> bubble-tea@gmail.com</p>
                    <div class="linkedin">
                      <img src="../static/img/linkedin.svg" alt="Italian Trulli" />
                      <p class="linkedin-text">bubble-tea.linkedinprofile.com</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      </div>
    </main>
    <footerNormal></footerNormal>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>


<script>

import imageHeader from '../components/imageHeader.vue'
import footerNormal from '../components/footerNormal.vue'
export default {
  name: "Images",
  components: {imageHeader,
            footerNormal},
  data() {
      return {
    objects: [
      {
        name: "Dog???",
        title: "Owner",
        image: [require("../static/img/dog1.jpeg")],
        Experience: "20 years",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
      {
        name: "Cat 2",
        title: "Founder",
        image: [require("../static/img/cat2.jpeg")],
        Experience: "15 years",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
      {
        name: "Evil Cat",
        title: "Accounting",
        image: [require("../static/img/cat3.jpeg")],
        Experience: "5 years",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
      {
        name: "Cat ???",
        title: "HR",
        image: [require("../static/img/cat4.jpeg")],
        Experience: "3 years",
        Bio:
          "Lorem ipsum dolor sit amet, consectetur...adipiscing elit, sed do eiusmod tempor incididunt utlabore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu",
      },
    ],
      }
  }
};
</script>


<style>
.body-container {
  margin: 1em;
  margin-right: 10em;
  margin-left: 10em;
  text-align: center;
}
.top-menu {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.nuxt-link {
  padding: 1em;
}
.button {
  background-color: #4caf50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 0.5em;
  cursor: pointer;
}

@media only screen and (min-width: 0px) {
  .body-container {
    margin: 0em;
    margin-right: 0em;
    margin-left: 0em;
    text-align: center;
  }
}

@media only screen and (min-width: 768px) {
  .body-container {
    margin: 1em;
    margin-right: 15em;
    margin-left: 15em;
    text-align: center;
  }
}

@media only screen and (min-width: 2000px) {
  .body-container {
    margin: 1em;
    margin-right: 40em;
    margin-left: 40em;
    text-align: center;
  }
}

.jumbotron {
  background-image: url("../static/img/blossoms.jpg");
  background-size: cover;
  display: flex;
  flex-direction: column;
  text-align: center;
}

.header-container {
  margin: 1em;
}

.top-menu {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.footer-container {
  padding: 5em;
  background-color: rgb(59, 42, 133);
}

.personimg {
  width: 100%;
  object-fit: cover;
  border-radius: 50%;
}
p {
  color: dimgray;
  text-align: center;
  font-size: 14px;
  padding: 0em;
  margin: 0em;
}

.titlename {
  color: lightgrey;
  text-align: center;
  font-size: 14px;
  padding: 0em;
  margin: 0em;
  font-style: italic;
}

.c1 {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  justify-content: space-between;
  margin: 0.5em;
  width: 33%;
}

.c2 {
  display: flex;
  align-items: left;
  justify-content: center;
  background-color: #f5f5f5;;
  flex-wrap: wrap;
  flex-direction: column;
  justify-content: center;
  margin: 1em;
  opacity: 0.9;
  width: 67%;
}

.linkedin {
  display: flex;
  width: 25%;
  flex-direction: row;
  vertical-align: baseline;
  padding-top: 1em;
}

.linkedin-text {
  font-size: 14px;
  padding: 0.2em;
  padding-top: 6px;
  padding-left: 4px;
  font-family: "Work Sans", sans-serif;
  color: black;
  font-weight: bolder;
  text-align: left;
  margin: 0em;
}

.card-text-box {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  background-color: whitesmoke;
  margin-left: 1em;
  margin-right: 1em;
  margin-top: 1em;
  margin-bottom: 1em;
  position: relative;
  opacity: 0.6;
}

.cardp {
  font-family: "Work Sans", sans-serif;
  font-size: 14px;
  color: black;
  text-align: left;
  margin: 0em;
  padding: 0.2em;
}
.card-instructor {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  transition: 0.3s;
  width: 100%;
  margin: 0em;
  margin-bottom: 0.5em;
}
</style>
