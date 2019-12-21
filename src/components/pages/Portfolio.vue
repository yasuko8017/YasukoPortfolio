<template>
  <div id='portfolio'>
    <div class="portfolioContent">
      <h2>
        PORTFOLIO
      </h2>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #portfolio{
    width: 100%;
    background: linear-gradient(to right, #FFFFFF, #DBEDF0);
    .portfolioContent{
      margin:0px auto;
      padding: 50px;
    }
  }
  // PC
  @media screen and (min-width: 1024px) {
    #portfolio{
      .portfolioContent{
        width: 960px;
        
      }
    }
  }
  // 手機 & 平板
  @media screen and (max-width: 1023px) {
    #portfolio{
      .portfolioContent{
        box-sizing: border-box;
        width: 100%;
      }
    }
  }
</style>