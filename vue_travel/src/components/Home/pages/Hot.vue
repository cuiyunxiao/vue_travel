<template>
  <div class="hot">
    <div class="hot-top">
      <img src="https://simg1.qunarzz.com/piao/images/sub_nav/hot.png" />
      <span>本周热门榜单</span>
      <span class="hot-title">全部榜单 ></span>
    </div>
    <ul class="hot-list" >
      <li class="hot-item" v-for="item in  hotList " :key="item.id">
        <img :src=" item.imgUrl">
        <p>{{item.title}}</p>
        <p>
          <span class="hot-mark">￥{{item.mark}}</span>起
        </p>
      </li>
    </ul>
  </div>
</template>

<script >
export default{
  data(){
    return{
      hotList:[
        {
          id:"01",
          imgUrl:"https://imgs.qunarzz.com/piao/fusion/2008/ac/22bba3766b2d5002.jpg_228x168_ddcd3452.jpg",
          title:'故宫',
           mark:'20'
        },
        {
          id:"02",
          imgUrl:"https://imgs.qunarzz.com/piao/fusion/2009/7f/503a90ac14a0b702.jpg_228x168_dc0075c2.jpg",
          title:'十度聚龙湾玻璃栈道',
           mark:'30'
        },
        {
          id:"03",
          imgUrl:"https://imgs.qunarzz.com/piao/fusion/2010/e2/90c63cf82df6eb02.jpg_228x168_3e1465a1.jpg",
          title:'颐和园',
           mark:'40'
        },
        {
          id:"04",
          imgUrl:"https://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/fusion/20197/06554d9bfa0a1cdcccca6652432e9b8e.jpg_228x168_11ed0f98.jpg",
          title:'金海湖风景区',
           mark:'50'
        },
       
        {
          id:"05",
          imgUrl:" https://imgs.qunarzz.com/sight/p0/201405/12/51b63883c25f5d87af3c08bb016e2bd7.jpg_250x250_6ec2f798.jpg",
          title:'恭王府',
           mark:'60'
        },
        {
          id:"06",
          imgUrl:"https://imgs.qunarzz.com/sight/p0/1602/92/920e47352552c1c990.water.jpg_250x250_ee99c18e.jpg",
          title:'天坛公园',
           mark:'50'
        },
      ]
    }
  }
}
</script>

<style scoped >
  .hot{
    margin-top:.2rem ;
    background: #fff;
    font-size:.28rem;
  }
  .hot-top{
   padding: .2rem;
  }
  .hot-top img{
    width:.3rem;
    height:.3rem;
  }
  .hot-top span{
    color: #212121;
    font-size: .32rem;
  }
.hot-title{
    position: absolute;
    right: .2rem;
    color:#616161;
    font-size:.28rem;
  }
.hot-list{
overflow-x: scroll;
white-space: nowrap;
overflow-y: hidden;
height: 3rem;
}
.hot-item{
    height:2rem ;
    width: 2rem;
    padding: 0 .2rem;
    display: inline-block;
    padding: .1rem;
}
.hot-item img{
 height:100% ;
   width:100%;
}
.hot-item p{
  text-align: center;
  margin-top: .1rem;
  white-space: nowrap;
  text-overflow :ellipsis;
  overflow : hidden;
}
.hot-item p .hot-mark{
  color:#ff8300;
 font-size: .32rem;

}

</style>
