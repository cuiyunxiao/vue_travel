<template>
  <div class="header">
  <div class="header-left">
    <span class='iconfont'>&#xe648;</span>
  </div>
   <div class="header-search">
     <span class='iconfont'>&#xe632;</span>
     输入城市/景点/游玩主题
   </div>
    <div class="header-right">
      广州
     <span class='iconfont'>
       &#xe64a;
     </span>
    </div>
  </div>
</template>

<script >
</script>

<style scoped>
  .header{
    width: 100%;
    height:.88rem;
    line-height: .88rem;
    background: #00bcd4;
    color:#fff;
    font-size: .36rem;
   display: flex;
  }
  .header-left{
    width: .4rem;
    padding: 0 .2rem;
    text-align: center;
    font-weight: bold;
  }
  .header-search{
    flex:1;
    background: #fff;
    height:.6rem;
    margin: .14rem  0;
    border-radius: .1rem ;
    color:#e4e7ea;
    line-height: .6rem;
    font-size: .28rem;
    padding-left:.2rem ;
  }
  .header-right{
    font-size: .28rem;
    padding: 0 .2rem;
  }
</style>
