<template>
  <div>
    <p>
      YASUKO  PORTFOLIO
    </p>
  </div>
</template>

<style lang="scss" scoped>
div{
  width: 100%;
  background: #7FC1D0;
  opacity:0.8;
  padding:20px 0;
  top:0;
  position:fixed;
  z-index: 9;
}
p{
  color: #ffffff;
  font-size: 1em;
  letter-spacing: 0.8em;
  padding-left: 50px;
}
// 手機 & 平板
@media screen and (max-width: 1023px) {
  div{
    padding:15px 0;
    text-align: center;
  }
  p{
    letter-spacing: 0.4em;
    font-size: 0.7em;
    padding-left: 0px;
  }
}
</style>