<template>
  <div id='about'>
    <div class="aboutContent">
      <div class="photo">
        <img src="../../assets/life.jpg" alt="生活照">
      </div>
      <div class="intro">
        <h2>
          ABOUT ME
        </h2>
        <div class="name">
          <p>陳靖安</p>
          <p>Tina Chen / Yasuko</p>
        </div>
        <p>走過了 6 年的 Full Stack Developer 瀑布 / 敏捷 軟體開發經驗，停下腳步，豁然發現自己離最初的目標漸行漸遠...</p>
        <p>28歲這年，給自己一個機會，努力學習前端技術，期望能早日成為一名專業的前端工程師</p>
        <p>期待與您合作的機會☺</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #about{
    width: 100%;
    background: #fff;
    .aboutContent{
      display: flex;
      margin:0px auto;
      .photo{
        img{
          border-radius:50%;
        }
      }
      .intro{
        padding: 50px;
        .name{
          font-weight: bold;
          color: #002D5E;
        }
        p{
          color: #002D5E;
        }
      }
    }
  }
  // PC
  @media screen and (min-width: 1024px) {
    #about{
      .aboutContent{
        width: 960px;
        .photo{
          width: 30%;
          padding: 30px;
        }
        .intro{
          box-sizing: border-box;
          width: 70%;
          .name{
            font-size: 1.5em;
            padding: 1em 0em;
          }
          p{
            font-size: 0.9em;
            line-height: 1.5em;
            display: inline;
            padding-right: 1em;
          }
        }
      }
    }
  }
  // Pad
  @media screen and (min-width: 768px) and (max-width: 1023px) {
    #about{
      .aboutContent{
        width: 80%;
        flex-direction: column;
        .photo{
          text-align: center;
          padding-top: 30px;
          img{
            width: 50%
          }
        }
        .intro{
          box-sizing: border-box;
          .name{
            font-size: 1.5em;
            padding: 1em 0em;
          }
          p{
            font-size: 0.9em;
            line-height: 1.5em;
          }
        }
      }
    }
  }
  // Mobile
  @media screen and (max-width: 767px) {
    #about{
      .aboutContent{
        width: 100%;
        flex-direction: column;
        .photo{
          margin: 50px auto 0px auto;
          width: 65%;
        }
        .intro{
          box-sizing: border-box;
          .name{
            font-size: 1.5em;
            padding: 1em 0em;
          }
          p{
            font-size: 0.9em;
            line-height: 1.5em;
          }
        }
      }
    }
  }
</style>