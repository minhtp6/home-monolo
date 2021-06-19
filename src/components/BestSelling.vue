<template>
  <span class="col">
    <td v-for="(item,key) in items" :item="item" :key="key" id="web" style="padding-right: 2pc">
        <img :src="item.img"/>
        <p class="title">{{item.title}}</p>
        <p class="price">{{item.price}}</p>
        <button>ADD TO CART</button>
    </td>
    
  </span>
</template>
<script>
export default {
  data() {
      return{
    items: [
      {
        title: "Plaid Long Sleeve Loose Crew Neck Plus Size Vintage Dress",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f56ac749aaeacb476f1.jpeg",
        price:"$28.97"
      },
       {
        title: "Vintage Women Solid 3/4 Sleeve Loose Maxi Dress For Women",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f567c2ee6ea1212709c.jpeg",
        price:"$28.97"
      },
       {
        title: "Vintage Floral Print Patchwork Long Sleeve Dress with Pockets",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f597c2ee65f9d1270c0.jpeg",
        price:"$28.97"
      },
       {
        title: "Women Floral Wrap Dress Off Shoulder Tie Up Front Ruffle Mini Dress Summer Office Lady Slash Neck Printed Pencil Dress",
        img: "https://minio.lattehub.com/img/310/300/resize/60bdc849e0db61849045908f/2021/06/10/latte-image-60c28f8c7c2ee62b24127279.jpeg",
        price:"$28.97"
      },
    ],}
  },
};
</script>
<style scoped lang='css'>
.col {
  display: inline-block;
  text-align: center;
  font-weight: bold;
  font-size: 120%;
  width: 65%;
  margin-left: 25%;
  margin-top: 0%;
  padding-top: 0%;
}
p{
    overflow: hidden;
}
.col td{
   width: 240px; 
   position: relative;
}
.col td:hover button{
    visibility: visible;
}
.col td img {
  width: 100%;
  height: 250px;
  margin-right: 10px;
}
.title{
    font-weight: normal !important;
    height: 50px;
    text-align: left;
    padding-left: 10px;
    font-size: 14px;
}
.price{
    color: lightskyblue !important;
    font-weight: normal !important;
    text-align: left;
    padding-left: 10px;
}
button{
  visibility: hidden;
  border: none;
  background-color: #0654f3 !important;
  color: white !important;
  font-size: 100% !important;
  font-weight: bold;
  width: 90%;
  height: 2.5pc;
  margin-top: 1%;
  margin-bottom: 3%;
}
@media screen and (max-width: 600px) {
    .col {
  display: flexbox;
  text-align: center;
  font-weight: bold;
  font-size: 120%;
  width: 100%;
  margin: 10px;
  overflow: hidden;
}
.col td{
   width: 180px; 
   height: 100px;
   display: flexbox;
}
.col td img {
  width: 150px;
  height: 150px;
  margin-right: 10px;
}
button{
    visibility: visible;
}
}
</style>