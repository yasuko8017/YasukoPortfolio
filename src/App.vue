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
    font-size: 2em;
    font-weight: bolder;
    letter-spacing: 0.3em;
    text-align: center;
    padding: 2.2em 0 1em 0;
    span{
      color: #8DABC5;
      padding: 15px 100px;
    }
  }
</style>