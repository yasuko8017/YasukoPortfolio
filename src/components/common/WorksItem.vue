<script>
export default {
  props: ['workdata'],
}
</script>

<template>
  <div class="work">
    <div class="image">
      <img :src="workdata.img" />
    </div>
    <div class="title">
      {{ workdata.title }}
    </div>
    <div class="description">
      {{ workdata.desc }}
    </div>
    <div class="btn">
      <a :href="workdata.codeUrl" class="codeBtn">
        <p>CODE</p>
      </a>
      <a :href="workdata.url" class="urlBtn">
        <p>URL</p>
      </a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.work {
  background: #dbedf0;
  box-shadow: 4px 4px 8px #80a491;
  border-radius: 5px;
  overflow: hidden;
  .image {
    background: #ffffff;
    width: 100%;
    overflow: hidden;
    img {
      display: block;
      margin: 0px auto;
    }
  }
  .title {
    color: #1760a0;
    text-align: center;
    padding: 15px;
    white-space: nowrap;
    font-weight: bolder;
  }
  .description {
    padding: 0px 10px;
    color: #4699ca;
  }
  .btn {
    text-align: center;
    position: relative;
    a {
      display: block;
      background: #7fc1d0;
      color: #ffffff;
      font-weight: bolder;
      padding: 10px;
      position: absolute;
    }
    .codeBtn {
      bottom: 0;
      left: 0;
    }
    .urlBtn {
      bottom: 0;
      right: 0;
    }
  }
}
// PC
@media screen and (min-width: 1024px) {
  .work {
    width: 290px;
    margin: 15px;
    float: left;
    .image {
      padding-top: 10px;
      padding-bottom: 10px;
      height: 180px;
      img {
        height: 100%;
      }
    }
    .title {
      font-size: 1em;
    }
    .description {
      font-size: 0.8em;
      line-height: 1.5em;
      height: 90px;
    }
    .btn {
      a {
        width: 124px;
        font-size: 0.8em;
      }
    }
  }
}
// Pad
@media screen and (min-width: 768px) and (max-width: 1023px) {
  .work {
    width: 354px;
    margin: 15px;
    float: left;
    .image {
      box-sizing: border-box;
      padding-top: 10px;
      padding-bottom: 10px;
      height: 240px;
      img {
        height: 100%;
      }
    }
    .title {
      font-size: 0.9em;
    }
    .description {
      font-size: 0.65em;
      line-height: 1.5em;
      height: 90px;
    }
    .btn {
      a {
        width: 156px;
        font-size: 0.6em;
      }
    }
  }
}
// Mobile
@media screen and (max-width: 767px) {
  .work {
    width: 320px;
    margin: 15px auto;
    .image {
      padding-top: 8px;
      padding-bottom: 8px;
      img {
        width: 95%;
      }
    }
    .title {
      font-size: 0.9em;
    }
    .description {
      font-size: 0.65em;
      line-height: 1.5em;
      height: 80px;
    }
    .btn {
      a {
        width: 139px;
        font-size: 0.6em;
      }
    }
  }
}
</style>
