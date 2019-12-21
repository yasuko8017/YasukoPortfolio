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
  top: 30%;
  z-index: 9;
  li{
    width: 80px;
    font-size: 1em;
    font-weight:500;
    text-align: center;
    align-self: auto;
    padding: 20px 10px;
    margin-top: 2px;
    background: #7FC1D0;
    opacity:0.6;
    a{
      color: #fff;
    }
  }
  li:hover{
    width: 100px;
    opacity:1;
    text-align: right;
    padding-right: 30px;
    a{
      color: #fff;
    }
  }
}
</style>