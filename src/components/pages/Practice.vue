<script>
import WorksList from '../common/WorksList';
import practiceWorks from "../../data/practiceWorks";

export default {
  computed:{
    practiceWorks(){
      return practiceWorks;
    }
  },
  components:
  {
    WorksList,
  }
}
</script>

<template>
  <div id='practice'>
    <div class="practiceContent">
      <h2>
        PRACTICE
      </h2>
      <WorksList :works="practiceWorks"/>
      <h3>
        課程學習上的一些小練習或是作業
      </h3>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #practice{
    width: 100%;
    background: linear-gradient(to right, #FFFFFF, #DBEDF0);
    .practiceContent{
      margin:0px auto;
      h3{
        font-weight: bolder;
        color: #7FC1D0;
      }
    }
  }
  // PC
  @media screen and (min-width: 1024px) {
    #practice{
      .practiceContent{
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
    #practice{
      .practiceContent{
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
    #practice{
      .practiceContent{
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