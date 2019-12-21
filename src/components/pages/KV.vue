<template>
  <div id='kv'>
    <div>
      <h1>I'M YASUKO</h1>
      <div class="role">
        <p>A FULL STACK DEVELOPER</p> 
        <p>& GONNA BE A <span>FRONTEND DEVELOPER</span></p>
      </div>
      <div class="icons">
        <a href="https://www.facebook.com/ChenYasuko"><font-awesome-icon :icon="['fab', 'facebook']" size="lg" style="color:#4A8060"/></a>
        <a href="https://www.linkedin.com/in/yasuko-chen-479584b3/"><font-awesome-icon :icon="['fab', 'linkedin-in']" size="lg" style="color:#4A8060"/></a>
        <a href="https://github.com/yasuko8017"><font-awesome-icon :icon="['fab', 'github']" size="lg" style="color:#4A8060"/></a>
        <a href="https://codepen.io/yasukochen"><font-awesome-icon :icon="['fab', 'codepen']" size="lg" style="color:#4A8060"/></a>
      </div>
    </div>
    <img class="yasuko" src="../../assets/yasuko.png" alt="yasuko photo">
  </div>
</template>

<style lang="scss" scoped>
  #kv {
    height: 700px;
    width: 100%;
    background: linear-gradient(60deg, #DBEDF0 35%, #fff, #80A491);
    position: relative;
    z-index: 0;
    .yasuko {
      right: 50px;
      height: 600px;
      position: absolute;
      bottom: 0;
      z-index: 0;
    }
    h1 {
      color: #002D5E;
      font-size: 3em;
      font-weight: bolder;
      letter-spacing: 0.1em;
      position: absolute;
      top: 300px;
      left: 300px;
    }
    .role{
      position: absolute;
      top: 370px;
      left: 300px;
      line-height: 1.8em;
      p{
        color: #002D5E;
        opacity:0.5;
        font-size: 1.2em;
        font-weight: bold;
      }
      p span{
        color: red;
      }
    }
    .icons{
      position: absolute;
      top: 450px;
      left: 300px;
      a{
        display: inline;
        margin-right: 5px;
      }
    }
  }
</style>