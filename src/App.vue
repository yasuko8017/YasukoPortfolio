<script>
import SideMenu from './components/SideMenu.vue';
import Header from './components/Header.vue';
import KV from './components/pages/KV.vue';
import About from './components/pages/About.vue';
import Contact from './components/pages/Contact.vue';
import Portfolio from './components/pages/Portfolio.vue';
import Practice from './components/pages/Practice.vue';
import Footer from './components/pages/Footer.vue';

export default {
  components: {
    Header,
    SideMenu,
    KV,
    About,
    Contact,
    Portfolio,
    Practice,
    Footer,
  },
};
</script>

<template>
  <div>
    <Header/>
    <SideMenu/>
    <KV/>
    <About/>
    <Contact/>
    <Portfolio/>
    <Practice/>
    <Footer/>
</div>
</template>

<style lang="sass" src="./style/reset.sass"></style>
<style lang="scss">
  body{
    font-family: "Helvetica", "Arial","LiHei Pro","黑體-繁","微軟正黑體", sans-serif;
  }
  h2{
    font-weight: bolder;
    text-align: center;
    color: #8DABC5;
  }
  // PC
  @media screen and (min-width: 1024px) {
    h2{
      font-size: 1.7em;
      letter-spacing: 0.3em;
      padding-bottom: 0.6em;
    }
  }
  // Pad
  @media screen and (min-width: 768px) and (max-width: 1023px) {
    h2{
      font-size: 1.5em;
      letter-spacing: 0.3em;
      padding-bottom: 0.6em;
    }
  }
  // Mobile
  @media screen and (max-width: 767px) {
    h2{
      font-size: 1.5em;
      letter-spacing: 0.3em;
      padding-bottom: 0.6em;
    }
  }
</style>