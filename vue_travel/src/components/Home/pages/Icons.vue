<template>
  <div class="icons">
    <swiper :options="swiperOption" ref="mySwiper">
      <swiper-slide  v-for='(item,key) in page' :key='key'>
      <div class="icons-item" v-for='page in item'>
        <img :src="page.imgUlr" />
        <p>{{page.title}}</p>
      </div>
      </swiper-slide>

    </swiper>



  </div>
</template>

<script >
  export default{
    data(){
      return{
        swiperOption:{},
        iconsList:[
          {
            id:'01',
            imgUlr:"http://s.qunarzz.com/homenode/images/touchheader/piao.png",
            title:"景点门票"
          },
          {
            id:'02',
            imgUlr:"http://s.qunarzz.com/homenode/images/touchheader/hotel.png",
             title:"酒店"
          },
          {
            id:'03',
            imgUlr:"http://s.qunarzz.com/homenode/images/touchheader/flight.png",
             title:"机票"
          },
          {
            id:'04',
            imgUlr:"http://s.qunarzz.com/homenode/images/touchheader/train.png",
             title:"火车票"
          },
          {
            id:'05',
            imgUlr:"http://s.qunarzz.com/homenode/images/touchheader/package.png",
             title:"度假"
          },
          {
            id:'06',
            imgUlr:"https://picbed.qunarzz.com/1316dc82d1ce6259686d5a68880e5a9d.png",
             title:"攻略"
          },
          {
            id:'07',
            imgUlr:"https://picbed.qunarzz.com/ae617a31e0bd5803d76918b817f6d942.png",
             title:"自由行"
          },
          {
            id:'08',
            imgUlr:"https://picbed.qunarzz.com/a36d2288f19e54562338f4d8ef986288.png",
             title:"低价机票"
          },
          {
            id:'09',
            imgUlr:"https://picbed.qunarzz.com/f5e5770393d759578962e53ee67798c8.png",
             title:"海外酒店"
          },
          {
            id:'10',
            imgUlr:"https://picbed.qunarzz.com/01d2f57f920666364197a850dab859a8.png",
             title:"民宿客栈"
          },
        ]
      }

    },
    computed:{
      page(){
        let pages = [];
        this.iconsList.forEach((item,index)=>{
         let idx = Math.floor(index/8);//向下取整
         if(!pages[idx]) pages[idx] = [];
         pages[idx].push(item)

        })
        return pages;
      }
    }
  }

</script>

<style scoped>
  .icons{
    width: 100%;
    overflow: hidden;
  }
  .icons-item{
    width: 25%;
    padding-bottom: 25%;
    height: 0;
    float: left;
    }
    .icons-item img{
      width: 1.1rem;
      height: 1.1rem;
      display: block;
      margin: 0 auto;
      padding-top: .2rem;
    }
    .icons-item p{
      font-size: .28rem;
      text-align: center;
      color:#212121;
      margin-top: .1rem;
    }
</style>
