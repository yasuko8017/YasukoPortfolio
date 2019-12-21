<template>
  <div id='contact'>
    <div class="contactContent">
      <h2>
        CONTACT
      </h2>
      <div class="contact">
        <div class="icon">
          <font-awesome-icon :icon="['fas', 'address-card']" size="4x" style="color:#80A491"/>
        </div>
        <div class="content">
          <p>yasuko8017@hotmail.com</p>
          <p>Keelung</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #contact{
    width: 100%;
    background: linear-gradient(to right, #FFFFFF, #DBEDF0, #FFFFFF);
    .contactContent{
      margin:0px auto;
      padding: 50px;
      .contact{
        .content{
          color: #002D5E;
        }
      }
    }
  }
  // PC
  @media screen and (min-width: 1024px) {
    #contact{
      .contactContent{
        width: 960px;
        .contact{
          width: 50%;
          display: flex;
          margin:10px auto;
          .icon{
            text-align: right;
            width: 40%;
          }
          .content{
            width: 60%;
            font-size: 1em;
            line-height: 1.5em;
            padding-top: 0.4em;
            padding-left: 2em;
          }
        }
      }
    }
  }
  // 手機 & 平板
  @media screen and (max-width: 1023px) {
    #contact{
      .contactContent{
        box-sizing: border-box;
        width: 100%;
        .contact{
          width: 50%;
          display: flex;
          margin-top:10px;
          .icon{
            text-align: right;
            width: 40%;
          }
          .content{
            width: 60%;
            font-size: 1em;
            line-height: 1.5em;
            padding-top: 0.4em;
            padding-left: 2em;
          }
        }
      }
    }
  }
</style>