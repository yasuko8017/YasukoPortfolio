<script>
import axios from 'axios';

export default {
  data(){
    return {
      works: [
        {
          img: require("../../assets/works/portfolio.png"),
          title: "[Vue] 個人 Profolio",
          desc: "首次使用Vue.js做自主實作訓練，搭配sass實作RWD網頁(目前為初版，持續更新完善)",
          codeUrl: "https://github.com/yasuko8017/YasukoPortfolio",
          url: "https://yasuko8017.github.io/"
        },
        {
          img: require("../../assets/works/namecard.png"),
          title: "[排版] 名片實作",
          desc: "六角學院課堂實作，練習html及css的相對/絕對位置排版技巧",
          codeUrl: "https://codepen.io/yasukochen/pen/WNbbyJK",
          url: "https://codepen.io/yasukochen/pen/WNbbyJK"
        },
        {
          img: require("../../assets/works/votejoinrwd.png"),
          title: "[RWD] 集保投票活動頁面",
          desc: "2016年初，因應集保e票通專案，首次摸索/開發RWD頁面，開發APP內嵌集點活動頁面",
          codeUrl: "https://github.com/yasuko8017/VoteJoinRWD",
          url: "https://vote-join-rwd.herokuapp.com/index.html"
        },
      ],
      //url: window.location.href,
      //baseUrl: process.env.url,
    };
  },
  //mounted(){
  //  axios.get('../../data/portfolioWorks.json')
  //    .then(rs => this.works = rs.data);
  //},
  //methods: {
  //  imgStyle(img){
  //    return {
  //      backgroundImage: `url(${img})`,
  //      backgroundSize: 'cover',
  //    }
  //  }
  //},
}
</script>

<template>
  <div id='portfolio'>
    <div class="portfolioContent">
      <h2>
        PORTFOLIO
      </h2>
      <div class="worksContent">
        <div v-for="work in works" class="work"> 
          <!--<img :src="work.img"/>-->
          <!--<div class="image" :style="imgStyle(work.img)"></div>-->
          <div class="image">
            <img :src="work.img"/>
          </div>
          <div class="title">
            {{work.title}}
          </div>
          <div class="description">
            {{work.desc}}
          </div>
          <div class="btn">
            <a :href="work.codeUrl" class="codeBtn">
              <p>CODE</p>
            </a>
            <a :href="work.url" class="urlBtn">
              <p>URL</p>
            </a>
          </div>
        </div>
        <div style="clear:both"></div>
      </div>
      <h3>
        近日來努力精進自己的前端技能，邊學習邊實作，作品集持續開發進行中
      </h3>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #portfolio{
    width: 100%;
    background: linear-gradient(to right, #FFFFFF, #DBEDF0);
    .portfolioContent{
      margin:0px auto;
      .worksContent{
        width: 100%;
        .work{
          background: #DBEDF0;
          box-shadow:4px 4px 8px #80A491;
          border-radius: 5px;
          overflow: hidden;
          .image{
            background: #FFFFFF;
            width: 100%;
            overflow: hidden;
            img{
              display: block;
              margin:0px auto;
            }
          }
          .title{
            color: #1760A0;
            text-align: center;
            padding: 15px;
            white-space:nowrap;
            font-weight: bolder;
          }
          .description{
            padding: 0px 10px;
            color: #4699CA;
          }
          .btn{
            text-align: center;
            position: relative;
            a{
              display: block;
              background: #7FC1D0;
              color: #FFFFFF;
              font-weight: bolder;
              padding: 10px;
              position: absolute;
            }
            .codeBtn{
              bottom: 0;
              left: 0;
            }
            .urlBtn{
              bottom: 0;
              right: 0;
            }
          }
        }
      }
      h3{
        font-weight: bolder;
        color: #7FC1D0;
      }
    }
  }
  // PC
  @media screen and (min-width: 1024px) {
    #portfolio{
      .portfolioContent{
        width: 960px;
        padding: 50px;
        .worksContent{
          .work{
            width: 290px;
            margin: 15px;
            float: left;
            .image{
              padding-top: 10px;
              padding-bottom: 10px;
              height: 180px;
              img{
                height: 100%;
              }
            }
            .title{
              font-size: 1em;
            }
            .description{
              font-size: 0.8em;
              line-height: 1.5em;
              height: 90px;
            }
            .btn{
              a{
                width: 124px;
                font-size: 0.8em;
              }
            }
          }
        }
        h3{
          font-size: 0.8em;
          letter-spacing: 0.1em;
          padding-top: 1em;
          padding-left: 15px;
        }
      }
    }
  }
  // Pad
  @media screen and (min-width: 768px) and (max-width: 1023px) {
    #portfolio{
      .portfolioContent{
        width: 768px;
        .worksContent{
          .work{
            width: 354px;
            margin: 15px;
            float: left;
            .image{
              box-sizing: border-box;
              padding-top: 10px;
              padding-bottom: 10px;
              height: 240px;
              img{
                height: 100%;
              }
            }
            .title{
              font-size: 0.9em;
            }
            .description{
              font-size: 0.65em;
              line-height: 1.5em;
              height: 90px;
            }
            .btn{
              a{
                width: 156px;
                font-size: 0.6em;
              }
            }
          }
        }
        h3{
          font-size: 0.8em;
          letter-spacing: 0.1em;
          padding-top: 1em;
          padding-left: 15px;
        }
      }
    }
  }
  // Mobile
  @media screen and (max-width: 767px) {
    #portfolio{
      .portfolioContent{
        box-sizing: border-box;
        padding-top: 50px;
        .worksContent{
          width: 100%;
          display: flex;
          flex-direction: column;
          .work{
            width: 320px;
            margin:15px auto;
            .image{
              padding-top: 8px;
              padding-bottom: 8px;
              img{
                width: 95%;
              }
            }
            .title{
              font-size: 0.9em;
            }
            .description{
              font-size: 0.65em;
              line-height: 1.5em;
              height: 80px;
            }
            .btn{
              a{
                width: 139px;
                font-size: 0.6em;
              }
            }
          }
        }
        h3{
          font-size: 0.8em;
          letter-spacing: 0.1em;
          line-height: 1.5em;
          padding: 15px 20px 40px 20px;
        }
      }
    }
  }
</style>