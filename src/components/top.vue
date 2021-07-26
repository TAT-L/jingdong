<template>
  <div class="top">
    <div class="tl"></div>
    <div class="slide1" >
      <slide :pics="item1" height="480px" img="true"></slide>
    </div>
    <div class="slide2">
      <slideMin :slides="item2" :img=true></slideMin>
    </div>
    <div class="tr"></div>
  </div>
</template>

<script>

import slide from './slide.vue'
import slideMin from './slideMin.vue'

export default {
    name:"top",
     components: {
        slide,
        slideMin
    },
    data() {
        return {
          img:true,
            item1:[
                {
                  url:  'https://imgcps.jd.com/img-cubic/creative_server_cia/v2/2000366/35211725905/FocusFullshop/CkNqZnMvdDEvMzYyOTYvMTkvMTU0ODkvMzU2NjY0LzYwZTZiODVhRWRiZWE4ZDk2L2Y3MThiOGMxYjRlMWIyYmUucG5nEgkyLXR5XzBfNTMwAjjui3pCEwoP6IKW5LiJ5amG5YWU6IKJEABCDgoK5ruhNDjlh48xMBABQhAKDOeri-WNs-aKoui0rRACQgoKBueyvumAiRAHWNGYoZaDAQ/cr/s/q.jpg' ,
                },
                {
                    url:'https://imgcps.jd.com/ling4/26849669333/57uZ5L2g5a625p2l54K56aKc6Imy/5aW954mp5L2O6IezOS455YWDIQ/p-5bd8253082acdd181d02fa17/ec6ec332/cr/s/q.jpg'
                },
                {
                    url:'https://img20.360buyimg.com/babel/s1180x940_jfs/t1/186079/20/14595/101187/60f4efb2E39bc31c1/061bf24f4ac76b73.jpg.webp'
                }
            ]  ,
            item2: [
                   [
                      {
                        url:"https://img10.360buyimg.com/da/s380x300_jfs/t1/111591/13/1474/70016/5e98290bEfc6f7cc1/9988f24a2797dba5.png.webp",
                      },
                      {
                        url:"https://img30.360buyimg.com/babel/s380x300_jfs/t1/174099/26/10674/72264/60a61062Ea28b0c95/c0ac442553b76cb1.jpg.webp",
                      }
                   ],
                  [
                      {
                          url: "https://img14.360buyimg.com/babel/s380x300_jfs/t1/168591/2/9328/64891/603ddb1aE93567699/3e4e717eeac051b2.jpg.webp"
                      },
                      {
                          url:"https://img12.360buyimg.com/babel/s380x300_jfs/t1/152314/13/19839/57522/603e118dE941f0ce9/fdff58457adbef3e.jpg.webp"
                      }
                  ],
                      [
                          {
                              url:"https://img12.360buyimg.com/da/s380x300_jfs/t1/89744/32/18887/37792/5e9a2da9Ea04345da/695604c44e477e63.png.webp"
                          },
                          {
                              url:"https://img11.360buyimg.com/babel/s380x300_jfs/t1/181595/29/5122/90113/60a611c2Edbe5dcf2/38aec127b8a2a488.jpg.webp"
                          },
                      ],         
           ]
        }
    }  
  }  
    
</script>

<style>
.top {
  background-color: var(--gray-bg);
  height: 480px;
  position: relative;
  border: 1px solid rgb(122, 174, 194);
  display: flex;
}

.tl {
  margin-right: 10px;
  width: 17%;
  height: 100%;
  background-color: #fff;
}

.slide1 {
  margin-right: 10px;
  width: 49%;
  border: 1px solid red;
  height: 100%;
}

.slide2 {
  margin-right: 10px;
  width: 15%;
  border: 1px solid rgb(132, 65, 125);
  height: 100%;
}
.tr {
  border: 1px solid red;
  height: 100%;
}
</style>

