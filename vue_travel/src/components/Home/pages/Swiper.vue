<template>
  <div class="header-swiper">
   <swiper :options="swiperOption" ref="mySwiper">
       <!-- slides -->
       <swiper-slide>
         <img src="https://m.tuniucdn.com/fb2/t1/G5/M00/A0/2E/Cii-tFxuVYmIGWTZAD5OhK3A1yIAAUAZwCeOEIAPk6c476_w320_h180_c1_t0.jpg" />
       </swiper-slide>
       <swiper-slide>
         <img src="https://m.tuniucdn.com/fb2/t1/G5/M00/B7/0C/Cii-tFrNviKIBd5QAAikVCfoKoMAAFdVQJdjl8ACKRs115_w320_h180_c1_t0.jpg" />
       </swiper-slide>
       <swiper-slide>
           <img src="https://m.tuniucdn.com/fb2/t1/G4/M00/44/3A/Cii_J1z03rGIb1sqABbQpHGS-bsAAGrpwCVyLUAFtC8647_w320_h180_c1_t0.jpg" />
       </swiper-slide>
       <swiper-slide>
           <img src="https://m.tuniucdn.com/fb2/t1/G1/M00/97/59/Cii9EVi6Z0aIf_K_ADKuK1tJ_D0AAIU2wFIzOYAMq5D769_w320_h180_c1_t0.jpg" />
       </swiper-slide>

       <!-- Optional controls -->
       <div class="swiper-pagination"  slot="pagination"></div>

     </swiper>
  </div>
</template>

<script type="text/javascript">
  export default{
    data () {
      return {
        swiperList:[
          {
            id:'01',
            imgUrl:'https://m.tuniucdn.com/fb2/t1/G5/M00/A0/2E/Cii-tFxuVYmIGWTZAD5OhK3A1yIAAUAZwCeOEIAPk6c476_w320_h180_c1_t0.jpg'
          },
          {
            id:'01',
            imgUrl:'https://m.tuniucdn.com/fb2/t1/G5/M00/B7/0C/Cii-tFrNviKIBd5QAAikVCfoKoMAAFdVQJdjl8ACKRs115_w320_h180_c1_t0.jpg'
          },
          {
            id:'01',
            imgUrl:'https://m.tuniucdn.com/fb2/t1/G4/M00/44/3A/Cii_J1z03rGIb1sqABbQpHGS-bsAAGrpwCVyLUAFtC8647_w320_h180_c1_t0.jpg'
          },
          {
            id:'01',
            imgUrl:'https://m.tuniucdn.com/fb2/t1/G1/M00/97/59/Cii9EVi6Z0aIf_K_ADKuK1tJ_D0AAIU2wFIzOYAMq5D769_w320_h180_c1_t0.jpg'
          },
        ],
        swiperOption: {
          pagination: {
            el:'.swiper-pagination'
          },
          loop:true
         }
      }
    }
  }

</script>

<style type="text/css" scoped >
  .header-swiper{
    width: 100%;
    height:2.5rem;

  }
   .header-swiper img{
      width: 100%;
      height:2.5rem;
    }

</style>
