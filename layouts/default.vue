<template>
  <div>
    <Header />
    <Nuxt />
    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
    <Spacer />
    <Contact />
    <Spacer />
    <Footer />
  </div>
</template>

<script lang="ts">
import Header from '../components/Header.vue'
import Contact from '../components/Contact.vue'
import Footer from '../components/Footer.vue'
import Spacer from '../components/Spacer.vue'
import{ init } from 'emailjs-com';
init("user_xxN34oimmfOr9qeC0d3UU");

export default {
  name: "App",
  components: {
    Header,
    Contact,
    Footer,
    Spacer
  }
};
</script>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  height: 100%;
}
h1 {
  color: azure;
  text-align: center;
}
body {
  position: absolute;
  width: 100%;
  height: 25%;
  background-image: url('https://cdn.pixabay.com/photo/2019/11/14/13/01/abstract-4626113_960_720.jpg');
  background-size: cover;
  background-position: center;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #57bd6d;
  color: #57bd6d;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

html, body {
  margin: 0;
  height: 100%;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100%;
}

#footer {
  background-color: rgb(162, 160, 160);
  min-width: 100%;
}
img {
  width: 20px;
}

.footer {
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 60px;
    line-height: 60px;
    background-color: #f5f5f5;
}

.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
</style>
