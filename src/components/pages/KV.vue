<template>
  <div id='kv'>
    <div class="roleContent">
      <div class="wording">
        <h1>I'M YASUKO</h1>
        <div class="role">
          <p>A FULL STACK DEVELOPER</p> 
          <p>& GONNA BE A <span>FRONTEND DEVELOPER</span></p>
        </div>
        <div class="icons">
          <a href="https://www.facebook.com/ChenYasuko">
            <font-awesome-icon :icon="['fab', 'facebook']" size="lg" style="color:#4A8060"/>
          </a>
          <a href="https://www.linkedin.com/in/yasuko-chen-479584b3/">
            <font-awesome-icon :icon="['fab', 'linkedin-in']" size="lg" style="color:#4A8060"/>
          </a>
          <a href="https://github.com/yasuko8017">
            <font-awesome-icon :icon="['fab', 'github']" size="lg" style="color:#4A8060"/>
          </a>
          <a href="https://codepen.io/yasukochen">
            <font-awesome-icon :icon="['fab', 'codepen']" size="lg" style="color:#4A8060"/>
          </a>
        </div>
      </div>
      <div class="photo">
        <img src="../../assets/yasuko.png" alt="yasuko photo">
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #kv {
    width: 100%;
    background: linear-gradient(60deg, #DBEDF0 30%, #fff, #80A491);
    .roleContent{
      display: flex;
      margin:0px auto;
      .wording{
        box-sizing: border-box;
        h1 {
          color: #002D5E;
          font-weight: bolder;
          letter-spacing: 0.1em;
          margin-bottom: 10px;
        }
        .role{
          p{
            color: #002D5E;
            opacity:0.5;
            font-size: 1.2em;
            font-weight: bold;
          }
          p span{
            color: red;
          }
        }
        .icons{
          a{
            display: inline;
            margin-right: 5px;
          }
        }
      }
      .photo {
        box-sizing: border-box;
        img{
          display: block;
        }
      }
    }
  }

  // PC
  @media screen and (min-width: 1024px) {
    #kv {
      .roleContent{
        width: 960px;
        flex-direction: row;
        .wording{
          width: 65%;
          margin-top: 300px;
          padding-left: 80px;
          h1 {
            font-size: 2.5em;
          }
          .role{
            line-height: 1.8em;
            margin-bottom: 15px;
            p{
              font-size: 1.2em;
            }
            p span{
              color: red;
            }
          }
        }
        .photo {
          width: 35%;
          img{
            margin-top: 180px;
          }
        }
      }
    }
  }
  // Pad
  @media screen and (min-width: 768px) and (max-width: 1023px) {
    #kv {
      .roleContent{
        width: 100%;
        flex-direction: row;
        .wording{
          width: 65%;
          margin-top: 200px;
          padding-left: 120px;
          h1 {
            font-size: 1.5em;
          }
          .role{
            line-height: 1.5em;
            margin-bottom: 10px;
            p{
              font-size: 1em;
            }
            p span{
              color: red;
            }
          }
        }
        .photo {
          width: 35%;
          display: block;
          margin-right: 30px;
          img{
            margin-top: 100px;
          }
        }
      }
    }
  }
  // Mobile
  @media screen and (max-width: 767px) {
    #kv {
      .roleContent{
        width: 100%;
        flex-direction: column-reverse;
        .wording{
          margin: 60px auto;
          h1{
            font-size: 1.5em;
          }
          .role{
            line-height: 1.5em;
            margin-bottom: 10px;
            p{
              font-size: 1em;
            }
          }
        }
        .photo {
          position: relative;
          height: 300px;
          margin-top: 120px;
          overflow: hidden;
          img{
            position: absolute;
            width: auto;
            height: 100%;
            bottom: 0;
            left: 50%;
            margin-left: -20%;
          }
        }
      }
    }
  }
</style>