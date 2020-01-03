<script>
import WorksItem from "./WorksItem";
import axios from "axios";

export default {
  data() {
    return {
      works: [
        {
          img: require("../../assets/works/portfolio.png"),
          title: "[Vue] 個人 Profolio",
          desc:
            "首次使用Vue.js做自主實作訓練，搭配sass實作RWD網頁(目前為初版，持續更新完善)",
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
          desc:
            "2016年初，因應集保e票通專案，首次摸索/開發RWD頁面，開發APP內嵌集點活動頁面",
          codeUrl: "https://github.com/yasuko8017/VoteJoinRWD",
          url: "https://vote-join-rwd.herokuapp.com/index.html"
        }
      ]
      //url: window.location.href,
      //baseUrl: process.env.url,
    };
  },
  components: {
    WorksItem,
  }
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
};
</script>

<template>
  <div class="worksContent">
    <WorksItem v-for="work in works" :workdata="work" />
    <div style="clear:both"></div>
  </div>
</template>

<style lang="scss" scoped>
.worksContent {
  width: 100%;
}
// PC
@media screen and (min-width: 1024px) {
}
// Pad
@media screen and (min-width: 768px) and (max-width: 1023px) {
}
// Mobile
@media screen and (max-width: 767px) {
  .worksContent {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
}
</style>
