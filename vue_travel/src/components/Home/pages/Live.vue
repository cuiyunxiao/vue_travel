<template>
  <div class="live">
    <div class="live-top">
      <img src="https://imgs.qunarzz.com/piao/fusion/1711/89/ebc329f16c55bb02.png" />
      <span>猜你喜欢</span>

    </div>
    <ul class="live-list" >
      <li class="live-item" v-for="item in  liveList " :key="item.id">
      <div class="live-img">
        <img   :src="item.imgUrl"  />
      </div>
      <div class="live-text">
        <div  class="live-title">
          {{item.title}}
        </div>
        <div  class="live-message">
          {{item.message}}
        </div>
        <div class="live-map">
         <span class="live-mark">￥<b>{{item.pre}}</b></span>起
          <span  class="live-item-map">{{item.map}}</span>
        </div>
      </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default{
    data(){
      return{
      liveList: [
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
          title: '故宫',
          message: '20',
          pre: '20',
          map: '20'
        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
          title: '故宫',
          message: '20',
          pre: '20',
          map: '20'
        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
          title: '故宫',
          message: '20',
          pre: '20',
          map: '20'
        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
          title: '故宫',
          message: '20',
          pre: '20',
          map: '20'
        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
          title: '故宫',
          message: '20',
          pre: '20',
          map: '20'
        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
          title: '故宫',
          message: '20',
          pre: '20',
          map: '20'
        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
          title: '故宫',
          message: '20',
          pre: '20',
          map: '20'
        }
      ]
    }
  }
}
</script>

<style scope>
  .live{
    margin-top: .2rem;
    font-size:.28rem;
    background: #fff;
    padding: 0 .2rem;
  }
  .live-top{
    font-size: .32rem;
    padding: .2rem 0;
  }
  .live-top img{
    width: .3rem;
    height: .3rem;
  }
  .live-item{
    position: relative;
    overflow: hidden;
    border-bottom: 1px solid #CCCCCC;
    width: 100%;
    padding: .2rem 0;
  }
  .live-img{
    float: left;
    overflow: hidden;
  }
  .live-img img{
    width: 2rem;
    height: 2rem;
  }
  .live-text{
    padding-left: .2rem;
    overflow: hidden;

  }
  .live-title{
    font-size: .36rem;
    color:#212121;
    margin-top: .4rem;
  }
  .live-message{
       margin-top: .3rem;
       font-size: .24rem;
       color:#616161;
  }
  .live-map{
       margin-top: .3rem;
         color:#616161;
           position: relative;
  }
  .live-mark{
    color:#ff8300;
  }
  .live-mark b{
   font-size:.45rem ;
  }
  .live-item-map{
    position: absolute;
    right: 0;
    top: .1rem;
    font-size: .28rem;
  }
</style>
