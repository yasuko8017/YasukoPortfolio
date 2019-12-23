<template>
  <div id='practice'>
    <div class="practiceContent">
      <h2>
        PRACTICE
      </h2>
      
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #practice{
    width: 100%;
    background: linear-gradient(to right, #DBEDF0 40%, #fff);
    .practiceContent{
      margin:0px auto;
      padding: 50px;
    }
  }
  // PC
  @media screen and (min-width: 1024px) {
    #practice{
      .practiceContent{
        width: 960px;
        
      }
    }
  }
  // Pad
  @media screen and (min-width: 768px) and (max-width: 1023px) {
    #practice{
      .practiceContent{
        box-sizing: border-box;
        width: 100%;
      }
    }
  }
  // Mobile
  @media screen and (max-width: 767px) {
    #practice{
      .practiceContent{
        box-sizing: border-box;
        width: 100%;
      }
    }
  }
</style>