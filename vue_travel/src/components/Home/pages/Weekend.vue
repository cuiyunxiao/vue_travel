<template>
  <div class="weekend">
    <div class="weekend-top">
      <span>周末去哪里</span>

    </div>
    <ul class="weekend-list" >
      <li class="weekend-item" v-for="item in  weekendList " :key="item.id">
      <div class="weekend-img">
        <img   :src="item.imgUrl"  />
      </div>
      <div class="weekend-text">
        <div  class="weekend-title">
          {{item.title}}
        </div>
        <div  class="weekend-message">
          {{item.message}}
        </div>

      </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default{
  data () {
    return {
      weekendList: [
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/source/1811/15/66f14e0fd6fbb.jpg_r_640x214_5d69f21d.jpg',
          title: '清远周边逛',
          message: '人人都有一双发现美的眼睛，身边的事物最熟悉不过，那你可曾发现了被人遗漏的美？',

        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/source/1811/b8/5d599bbdcf8b57.jpg_r_640x214_2ee055e3.jpg',
          title: '浮在海上的绿洲',
          message: '南国滨海之城，避寒胜地，有暖暖的阳光，海风习习，吃着海鲜逛逛老街多惬意啊',

        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/source/1812/fe/208e0360d686b8.jpg_r_640x214_7b9e6607.jpg',
          title: '粤西温泉',
          message: '自驾粤西，这里有最全最心仪的温泉池，环境优美，舒舒服服的泡个热汤，远离繁忙的工作',

        },
        {
          id: '01',
          imgUrl: 'https://imgs.qunarzz.com/sight/source/1602/9c/39c5ce9ff58609.jpg_r_640x214_efb90102.jpg',
          title: '广州泡汤圣地',
          message: '解压之地，放松自己，来一段轻松的旅程。',

        },


      ]
    }
  }
}

</script>

<style>
  .weekend{
    margin-top: .2rem;
    font-size:.28rem;
    background: #fff;
    padding: 0 .2rem;
  }
  .weekend-top{
    font-size: .32rem;
    padding: .2rem 0;
  }
  .weekend-top img{
    width: .3rem;
    height: .3rem;
  }
  .weekend-item{
    position: relative;
    overflow: hidden;
    border-bottom: 1px solid #CCCCCC;
    width: 100%;
    padding: .2rem 0;
  }
  .weekend-img{
   /* float: left; */
    overflow: hidden;
  }
  .weekend-img img{
    width: 100%;
    height: 3rem;
  }
  .weekend-text{
    padding-left: .2rem;
    overflow: hidden;

  }
  .weekend-title{
    font-size: .32rem;
    color:#212121;
    margin-top: .4rem;
  }
  .weekend-message{
       margin-top: .2rem;
       font-size: .24rem;
       color:#616161;
  }
  .weekend-map{
       margin-top: .3rem;
         color:#616161;
           position: relative;
  }
  .weekend-mark{
    color:#ff8300;
  }
  .weekend-mark b{
   font-size:.45rem ;
  }
  .weekend-item-map{
    position: absolute;
    right: 0;
    top: .1rem;
    font-size: .28rem;
  }
</style>
