<template>
  <div>
    <a v-on:><span class="material-icons" id="menu"> menu </span></a>
    <img
      src="https://minio.lattehub.com/img/600/744/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bdd1cef27e5925329a45c9.png"
      width="150pc"
    />
    <a href="#"
      ><button id="search-a">
        <i class="material-icons" id="search"> search </i>What are you searching
        for?
      </button></a
    >
    <i class="material-icons" id="bag"> shopping_bag </i>
    <hr />
    <nav class="nav">
      <ul>
        <li>
          <a href="#"
            >Beauty<span class="material-icons"> arrow_drop_down </span></a
          >
          <ul>
            <li><a href="#">Hair Care</a></li>
            <li><a href="#">Nail Art</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >Women's Accessories<span class="material-icons">
              arrow_drop_down
            </span></a
          >
          <ul>
            <li><a href="#">Jewelry & Accessories</a></li>
            <li><a href="#">Footwear & Accessories</a></li>
            <li><a href="#">Leggings</a></li>
            <li><a href="#">Bag & Accessories</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >Health Care<span class="material-icons"> arrow_drop_down </span></a
          >
          <ul>
            <li><a href="#">Health</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >Life Styles<span class="material-icons"> arrow_drop_down </span></a
          >
          <ul>
            <li><a href="#">Home Improvement</a></li>
            <li><a href="#">Toys</a></li>
          </ul>
        </li>
        <li>
          <a href="#"
            >About Us<span class="material-icons" style="color: white">
              arrow_drop_down
            </span></a
          >
        </li>
        <li>
          <a href="#"
            >Contract Us<span class="material-icons" style="color: white">
              arrow_drop_down
            </span></a
          >
        </li>
        <li>
          <a href="#"
            >FAQs<span class="material-icons" style="color: white">
              arrow_drop_down
            </span></a
          >
        </li>
      </ul>
    </nav>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang='css'>
#menu{
  display: none;
}
#search-a {
  border: 0.1pc solid;
  border-color: rgb(190, 188, 188);
  display: inline;
  width: 18%;
  text-align: left;
  background-color: white;
  height: 2.5pc;
  color: rgb(190, 188, 188);
  font-size: 100%;
}
#bag {
  margin: 0% 20%;
}
#search {
  padding-right: 10%;
}
img {
  padding-left: 26%;
  padding-right: 5%;
}
.nav {
  text-align: left;
  padding-left: 25%;
  margin-top: 0%;
}
a {
  text-decoration: none;
  text-align: left;
}

hr {
  border-color: rgb(248, 248, 248);
  margin-bottom: 0;
}
ul {
  list-style: none;
  margin: 0;
  padding-left: 0;
}

li {
  display: block;
  float: left;
  padding: 1rem;
  position: relative;
  text-decoration: none;
  transition-duration: 0.5s;
}

li a {
  color: #4f4f4f;
}
li a:hover {
  color: #6f93f5;
  cursor: pointer;
}
li:hover {
  cursor: pointer;
}

ul li ul {
  visibility: hidden;
  opacity: 0;
  min-width: 5rem;
  position: absolute;
  transition: all 0.5s ease;
  margin-top: 1rem;
  left: 0;
  display: none;
}

ul li:hover > ul,
ul li:focus-within > ul,
ul li ul:hover {
  visibility: visible;
  opacity: 1;
  display: block;
}

ul li ul li {
  clear: both;
  width: 100%;
}
ul li ul li:hover {
  background-color: gainsboro;
}
ul li ul li a:hover {
  color: #4f4f4f;
}

@media screen and (max-width: 600px) {
  #search-a {
    border: 0;
    overflow: hidden;
    height: 1.5pc;
    color: black;
    width: 10%;
  }
  #bag {
    margin: 0% 5%;
  }
  img {
    padding-left: 10%;
    padding-right: 5%;
  }
  ul {
    display: none;
  }
  #menu{
    display: inline;
    padding-left: 5%;
  }
}
</style>