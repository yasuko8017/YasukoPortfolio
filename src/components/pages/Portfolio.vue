<script>
import WorksList from '../common/WorksList';

export default {
  components:
  {
    WorksList,
  }
}
</script>

<template>
  <div id='portfolio'>
    <div class="portfolioContent">
      <h2>
        PORTFOLIO
      </h2>
      <WorksList/>
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
        padding: 50px;
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