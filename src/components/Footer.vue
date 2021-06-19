<template>
  <div>
    <footer>
      <div class="footer-gray">
        <div class="footer-custom">
          <div class="footer-lists">
            <div class="footer-list-wrap">
              <h3 class="ftr-hdr">
                <img
                  src="https://minio.lattehub.com/img/600/744/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bdd1cef27e5925329a45c9.png"
                  width="150pc"
                />
              </h3>
              <ul class="ftr-links-sub">
                <li>
                  <span
                    ><b>Address: </b>Room 611, Building 3, Hongye Building West
                    Residential Area, Longhua District, Haikou City, Hainan
                    Province</span
                  >
                </li>
                <li>
                  <span><b>Email: </b>support@monolom.com</span>
                </li>
              </ul>
            </div>
            <div class="footer-list-wrap">
              <h3 class="ftr-hdr">Our Policies</h3>
              <ul class="ftr-links-sub">
                <li>
                  <a href="#">Privacy policy</a>
                </li>
                <li>
                  <a href="#">Terms of services</a>
                </li>
                <li>
                  <a href="#">Refund policy</a>
                </li>
                <li>
                  <a href="#">Shipping policy</a>
                </li>
                <li>
                  <a href="#">DCMA</a>
                </li>
                <li>
                  <a href="#">DCMA Report</a>
                </li>
              </ul>
            </div>
            <div class="footer-list-wrap">
              <h3 class="ftr-hdr">Help Center</h3>
              <ul class="ftr-links-sub">
                <li>
                  <a href="#">Contact Us</a>
                </li>
                <li>
                  <a href="#">FAQs</a>
                </li>
                <li>
                  <a href="#">Cancel/Change Order</a>
                </li>
                <li>
                  <a href="#">support@monolom.com</a>
                </li>
                <li>
                  <a href="#">Mon - Sat: 9AM - 6PM EST</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <hr />
        <div class="footer-custom">
          <div class="footer-list-wrap"><p>&copy; 2021 Monolom.</p></div>
        </div>
      </div>
    </footer>
    <div id="footerMobile" class="overlay">
      <img
        src="https://minio.lattehub.com/img/600/744/resize/60bdc849e0db61849045908f/2021/06/07/lattehub-image-60bdd1cef27e5925329a45c9.png"
        width="200pc"
      />
      <div class="overlay-content">
        <li>
          <a href="#" v-on:click="openMiniContact()"
            ><p>Contact Us</p>
            <span class="material-icons"> expand_more </span></a
          >
          <ul id="contact">
            <span
              ><b>Address: </b>Room 611, Building 3, Hongye Building West
              Residential Area, Longhua District, Haikou City, Hainan
              Province</span
            >
            <p><b>Email: </b>support@monolom.com</p>
          </ul>
        </li>
        <li>
          <a href="#" v-on:click="openMiniPolicies()"
            ><p>Our Policies</p>
            <span class="material-icons"> expand_more </span></a
          >
          <ul id="policies">
            <a href="#" class="mini">Privacy policy</a>
            <a href="#" class="mini">Terms of services</a>
            <a href="#" class="mini">Refund policy</a>
            <a href="#" class="mini">Shipping policy</a>
            <a href="#" class="mini">DCMA</a>
            <a href="#" class="mini">DCMA Report</a>
          </ul>
        </li>
        <li>
          <a href="#" v-on:click="openMiniHelp()"
            ><p>Help Center</p>
            <span class="material-icons"> expand_more </span></a
          >
          <ul id="help">
            <a href="#" class="mini">Contact Us</a>
            <a href="#" class="mini">FAQs</a>
            <a href="#" class="mini">Cancel/Change Order</a>
            <a href="#" class="mini">support@monolom.com</a>
            <a href="#" class="mini">Mon - Sat: 9AM - 6PM EST</a>
          </ul>
        </li>
      </div>
      <div><p>&copy; 2021 Monolom.</p></div>
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    openMiniContact() {
      document.getElementById("contact").classList.toggle("show");
      if (document.getElementById("policies").classList.contains("show")) {
        document.getElementById("policies").classList.remove("show");
      }
      if (document.getElementById("help").classList.contains("show")) {
        document.getElementById("help").classList.remove("show");
      }
    },
    openMiniPolicies() {
      document.getElementById("policies").classList.toggle("show");
      if (document.getElementById("contact").classList.contains("show")) {
        document.getElementById("contact").classList.remove("show");
      }
      if (document.getElementById("help").classList.contains("show")) {
        document.getElementById("help").classList.remove("show");
      }
    },
    openMiniHelp() {
      document.getElementById("help").classList.toggle("show");
      if (document.getElementById("contact").classList.contains("show")) {
        document.getElementById("contact").classList.remove("show");
      }
      if (document.getElementById("policies").classList.contains("show")) {
        document.getElementById("policies").classList.remove("show");
      }
    },
  },
};
</script>
<style scoped lang="css">
#footerMobile {
  display: none;
}
.mini {
  font-size: 15px !important;
}
.show {
  display: block;
}
.overlay {
  z-index: 1;
  width: 100%;
  margin: 0;
  background-color: #f1f1f1;
  overflow-x: hidden;
  transition: 0.5s;
  text-align: center;
}

.overlay-content {
  position: relative;
  width: 100%;
  text-align: left;
  margin-top: 0%;
}
.overlay-content li a {
  margin-bottom: 2%;
  display: inline-block;
  width: 100%;
}
.overlay-content li a ul {
  background-color: #f1f1f1;
}
.overlay-content li a p {
  display: inline-block;

  width: 300px;
  margin: auto;
}
.overlay-content li a span {
  display: inline;
  margin-right: 0px;
  text-align: right;
}

.overlay a {
  padding: 8px;
  text-decoration: none;
  font-size: 20px;
  color: black;
  display: block;
  transition: 0.3s;
}
.overlay .closebtn {
  font-size: 40px;
  top: 15px;
  right: 35px;
}
.hidden {
  display: none;
}
.footer-gray {
  margin-top: 10%;
  background-color: white;
  width: 100%;
  margin-bottom: 0%;
}
.footer-custom {
  color: black;
  font: normal normal 12px/1.4 "HelveticaNeue-Light", "Helvetica Neue Light",
    "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;
  max-width: 100%;
  box-sizing: border-box;
  margin: 0 auto;
  padding-left: 25%;
}
hr {
  width: 50%;
}

.footer-custom:after {
  display: table;
  clear: both;
  content: "";
}

.footer-lists:after {
  display: table;
  clear: both;
  content: "";
}

.ftr-hdr {
  color: #000;
  font: 25px/1.4 "BebasNeueRegular", BebasNeue, "Bebas Neue", Arial, sans-serif;
  font-weight: bold;
  margin: 1em 0 0;
}

.footer-list-wrap {
  width: 25%;
  float: left;
  box-sizing: border-box;
}

.ftr-links-sub {
  padding: 0;
  margin: 0;
}

.ftr-links-sub:after {
  display: table;
  clear: both;
  content: "";
}

.ftr-links-sub li {
  display: block;
  list-style-type: none;
  margin: 0;
  padding: 3px 0;
  color: black;
  font: normal 16px "HelveticaNeue-Light", "Helvetica Neue Light",
    "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;
  width: 75%;
}

.footer-custom a,
.footer-custom a:link,
.footer-custom a:visited,
.ftr-links-sub li .link {
  text-decoration: none;
  color: black;
  padding: 5px 0;
  display: block;
}

.footer-custom .footer-legal a {
  display: inline;
}

.footer-custom a:hover,
.footer-custom a:active,
.ftr-links-sub li .link:hover {
  text-decoration: underline;
  color: black;
  cursor: pointer;
}
.footer-lists {
  width: 100%;
  float: left;
}
@media screen and (max-width: 600px) {
  .footer-gray {
    display: none;
  }
  #footerMobile {
    display: block;
    margin-bottom: 0%;
  }
  ul {
    display: none;
  }
}
</style>