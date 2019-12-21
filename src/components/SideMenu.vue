<template>
  <div id="side_menu">
    <ul>
      <li><a href="#kv">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#practice">Practice</a></li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
#side_menu{
  position: fixed;
  z-index: 9;
  li{
    font-weight:500;
    text-align: center;
    align-self: auto;
    margin-top: 2px;
    background: #7FC1D0;
    opacity:0.6;
    a{
      color: #fff;
    }
  }
  li:hover{
    opacity:1;
    text-align: right;
    padding-right: 30px;
    a{
      color: #fff;
    }
  }
}
// PC
@media screen and (min-width: 1024px) {
  #side_menu{
    top: 30%;
    li{
      width: 80px;
      font-size: 1em;
      padding: 20px 10px;
    }
    li:hover{
      width: 100px;
    }
  }
}
// Pad
@media screen and (min-width: 768px) and (max-width: 1023px) {
  #side_menu{
    top: 150px;
    li{
      width: 60px;
      font-size: 0.8em;
      padding: 15px 10px;
    }
    li:hover{
      width: 70px;
    }
  }
}
// Mobile
@media screen and (max-width: 767px) {
  #side_menu{
    width: 100%;
    margin-top: 42px; 
    ul{
      width: 100%;
    }
    li{
      display: inline-block;
      box-sizing: border-box;
      width: 19%;
      font-size: 0.8em;
      padding: 12px 0px;
      margin-top: 2px;
    }
    li:hover{
      text-align: center;
      padding-right: 0px;
    }
  }
}
</style>