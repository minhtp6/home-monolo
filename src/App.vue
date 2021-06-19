<template>
  <div id="app">
    <Header id="header" />
 
    <Banner v-bind:banner="banners[0]"/>
    <br>
    <b id="colection">Collection list</b>
    <Collection/>
    <br>
    <div class="barHome"><b class="titleHome">Best Selling</b><button class="buttonHome">VIEW MORE</button> </div>
    <BestSelling/>
    <br>
    <img src="https://minio.lattehub.com/img/2000/2000/resize/60bdc849e0db61849045908f/2021/06/11/lattehub-image-60c2dec02f33d2dfe21c6b17.png" height="15%" width="100%">
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Banner from "./components/Banner.vue";
import Collection from "./components/Collection.vue"
import BestSelling from "./components/BestSelling.vue"
export default {
  name: "App",
  components: {
    Header,
    Footer,
    Banner,
    Collection,
    BestSelling
  },
  data() {
    return {
      banners: [
        {
          title: "SIXTH COLLECTION",
          subTitle: "Be Sexier - Be deeper in relationship",
          img: "https://minio.lattehub.com/img/2000/2000/resize/60bdc849e0db61849045908f/2021/06/09/lattehub-image-60c09bdc5793c9149caa93e4.jpeg",
          has: "1"
        },
        {
          title: "",
          subTitle: "",
          img: "https://minio.lattehub.com/img/2000/2000/resize/60bdc849e0db61849045908f/2021/06/11/lattehub-image-60c2dec02f33d2dfe21c6b17.png",
          has: "0"
        },
      ],
    };
  },
};
</script>

<style>
#app div{
  margin-bottom: 2%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 0%;
  overflow-x: hidden;
}
#header {
  position: sticky;
}
#colection{
  text-align: center;
  padding-left: 45%;
  font-size: 200%;
  font-weight: bold;
}
.titleHome{
  padding-left: 25%;
  font-size: 180%;
}
.barHome{
  padding-top: 1%;
  padding-bottom: 0%;
  margin-bottom: 0%;
}
.buttonHome{
  margin-left: 36%;
  border: none;
  background-color: #0654f3 !important;
  color: white !important;
  font-size: 160% !important;
  font-weight: bold;
  width: 10%;
  height: 3pc;
}
img{
  padding: 0;
  margin: 0;
}
@media screen and (max-width: 600px) {
  #app{
    padding: 0;
    margin: 0;
  }
  #colection{
  font-weight: bold;
  text-align: center;
  padding-left: 25%;
  font-size: 200%;
}
.buttonHome{
  margin-left: 25%;
  border: none;
  background-color: #0654f3 !important;
  color: white !important;
  font-size: 100% !important;
  font-weight: bold;
  width: 50%;
  height: 2.5pc;
  margin-top: 1%;
}
.titleHome{
  padding-left: 30%;
  font-size: 180%;
}
}
</style>
