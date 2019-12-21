<template>
  <div id='about'>
    <img src="../../assets/life.jpg" alt="生活照">
    <div class="intro">
      <h2>
        <span>ABOUT ME</span>
      </h2>
      <div class="name">
        陳靖安 - Tina Chen / Yasuko
      </div>
      <p>走過了 6 年的 Full Stack Developer 瀑布 / 敏捷 軟體開發經驗，停下腳步，豁然發現自己離最初的目標漸行漸遠...</p>
      <p>28歲這年，給自己一個機會，努力學習前端技術，期望能早日成為一名專業的前端工程師</p>
      <p>期待與您合作的機會☺</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #about{
    height: 30em;
    width: 100%;
    background: #fff;
    position: relative;
    img{
      height: 400px;
      margin: 2.5em 18em;
      float: left;
    }
    .intro{
      padding: 0 20%;
      .name{
        font-size: 1.5em;
        font-weight: bold;
        color: #002D5E;
        padding: 0.8em 0em;
      }
      p{
        font-size: 0.9em;
        line-height: 1.5em;
        color: #002D5E;
      }
    }
  }
</style>