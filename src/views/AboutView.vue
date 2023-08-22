<template>
  <div>
    <section class="about-section">
      <div class="container">
        <div class="row">
          <div class="content-column col-lg-6 col-md-12 col-sm-12 order-2">
            <div class="inner-column">
              <div class="sec-title">
                <span class="title">About Us</span>
                <h2 class="text-capitalize">RUKA STAR INTERNATIONAL LIMITED</h2>
              </div>
              <div class="text">
                Ruka Star International Limited is an indigenous Nigerian
                Company duly registered with Corporate Affairs Commission. Our
                corporate office is located at 12 SHEM JOSHUA STREET Opposite
                TRADEFAIR Satellite Town Lagos. We deal on foods, natural Spices
                and other Agro Commodities. Our Foods and Spices are natural and
                100% organic.
              </div>
              <div class="text">
                They are pure, healthy and neatly processed, packaged and
                distributed nationwide to grocery shops, departmental stores and
                food marts. We also export to Europe, Asia, USA and other parts
                of Africa. Our range of food products are Palm Oil, Garri,
                Abacha(cassava flakes), Melon, Ogbono, Kilishi (Beef Jerky),
                Suya Pepper, Kuli kuli (Peanut Bars), Groundnut oil (kulikuli
                oil only), Cocoyam, flour Pap, flour Bambara/Okpa, flour Bambara
                seed, Fufu, flour Yam, flour Unripe plantain.
              </div>
              <div class="text">
                <h3>We provide Natural Spices such as:</h3>
                <br />
                Ginger powder, garlic powder, Tumeric Powder, Suya spice, Pepper
                soup spice etc
              </div>
              <div class="text">
                <h3>And Agro Commodities such as:</h3>
                <br />
                Cashew and Cocoa etc
              </div>
              <div class="btn-box">
                <a href="#" class="theme-btn btn-style-one">Contact Us</a>
              </div>
            </div>
          </div>

          <!-- Image Column -->
          <div class="image-column col-lg-6 col-md-12 col-sm-12">
            <div class="inner-column wow fadeInLeft">
              <figure class="image-1">
                <a href="#" class="lightbox-image" data-fancybox="images"
                  ><img
                    title="Ruka Star"
                    src="https://i.ibb.co/QP6Nmpf/image-1-about.jpg"
                    alt=""
                /></a>
              </figure>
            </div>
          </div>
        </div>
        <div class="sec-title">
          <h5>Our Strength</h5>
        </div>
        <div class="text">
          <h4>At our facilities we have the following:</h4>
          <ul>
            <li>1. State of the Art Infrastructure</li>
            <li>2. Dedicated and well trained workforce</li>
            <li>3. Global Partnership</li>
            <li>4. Local Experience</li>
            <li>5. Full understanding of healthy foods and spices</li>
          </ul>
        </div>
        <div class="sec-title mt-10">
          <h5>Our Ambition</h5>
        </div>
        <div class="text">
          To make rich and healthy African Foods and Spices easily accessible
          globally
        </div>
      </div>
    </section>

    <section>
      <Footer />
    </section>
  </div>
</template>

<script>
import Footer from "@/components/Footer.vue";

export default {
  name: "About",
  components: {
    Footer,
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
h1,
h2,
h3,
h4,
h5,
h6 a,
a:hover,
a:focus,
a:active {
  text-decoration: none;
  outline: none;
}

a,
a:active,
a:focus {
  color: #6f6f6f;
  text-decoration: none;
  transition-timing-function: ease-in-out;
  -ms-transition-timing-function: ease-in-out;
  -moz-transition-timing-function: ease-in-out;
  -webkit-transition-timing-function: ease-in-out;
  -o-transition-timing-function: ease-in-out;
  transition-duration: 0.2s;
  -ms-transition-duration: 0.2s;
  -moz-transition-duration: 0.2s;
  -webkit-transition-duration: 0.2s;
  -o-transition-duration: 0.2s;
}

ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
img {
  max-width: 100%;
  height: auto;
}

.sec-title {
  position: relative;
  z-index: 1;
  margin-bottom: 60px;
}

.sec-title .title {
  position: relative;
  display: block;
  font-size: 18px;
  line-height: 24px;
  color: #004d40;
  font-weight: 500;
  margin-bottom: 15px;
}

.sec-title h5 {
  position: relative;
  display: block;
  font-size: 20px;
  color: #004d40;
  font-weight: 600;
  padding-bottom: 18px;
}

.sec-title h2:before {
  position: absolute;
  content: "";
  left: 0px;
  bottom: 0px;
  width: 50px;
  height: 3px;
  background-color: #d1d2d6;
}

.sec-title .text {
  position: relative;
  font-size: 16px;
  line-height: 26px;
  color: #848484;
  font-weight: 400;
  margin-top: 35px;
}

.sec-title.light h2 {
  color: #ffffff;
}

.sec-title.text-center h2:before {
  left: 50%;
  margin-left: -25px;
}


.btn-style-one {
  position: relative;
  display: inline-block;
  font-size: 17px;
  line-height: 30px;
  color: #ffffff;
  padding: 10px 30px;
  font-weight: 600;
  overflow: hidden;
  letter-spacing: 0.02em;
  background-color: #004d40;
}

.btn-style-one:hover {
  background-color: #004d40;
  color: #ffffff;
}
.about-section {
  position: relative;
  padding: 120px 0 70px;
}

.about-section .sec-title {
  margin-bottom: 45px;
}

.about-section .content-column {
  position: relative;
  margin-bottom: 50px;
}

.about-section .content-column .inner-column {
  position: relative;
  padding-left: 30px;
}

.about-section .text {
  margin-bottom: 20px;
  font-size: 16px;
  line-height: 26px;
  color: #848484;
  font-weight: 400;
}

.about-section .list-style-one {
  margin-bottom: 45px;
}

.about-section .btn-box {
  position: relative;
}

.about-section .btn-box a {
  padding: 15px 50px;
}

.about-section .image-column {
  position: relative;
}

.about-section .image-column .text-layer {
  position: absolute;
  right: -110px;
  top: 50%;
  font-size: 325px;
  line-height: 1em;
  color: #ffffff;
  margin-top: -175px;
  font-weight: 500;
}

.about-section .image-column .inner-column {
  position: relative;
  padding-left: 80px;
  padding-bottom: 0px;
}
.about-section .image-column .inner-column .author-desc {
  position: absolute;
  bottom: 16px;
  z-index: 1;
  background: #004d40;
  padding: 10px 15px;
  left: 96px;
  width: calc(100% - 152px);
  border-radius: 50px;
}
.about-section .image-column .inner-column .author-desc h2 {
  font-size: 21px;
  letter-spacing: 1px;
  text-align: center;
  color: #fff;
  margin: 0;
}
.about-section .image-column .inner-column .author-desc span {
  font-size: 16px;
  letter-spacing: 6px;
  text-align: center;
  color: #fff;
  display: block;
  font-weight: 400;
}
.about-section .image-column .inner-column:before {
  content: "";
  position: absolute;
  width: calc(50% + 80px);
  height: calc(100% + 160px);
  top: -80px;
  left: -3px;
  background: transparent;
  z-index: 0;
  border: 44px solid #004d40;
}

.about-section .image-column .image-1 {
  position: relative;
}
.about-section .image-column .image-2 {
  position: absolute;
  left: 0;
  bottom: 0;
}

.about-section .image-column .image-2 img,
.about-section .image-column .image-1 img {
  box-shadow: 0 30px 50px rgba(8, 13, 62, 0.15);
  border-radius: 46px;
}

.about-section .image-column .video-link {
  position: absolute;
  left: 70px;
  top: 170px;
}

.about-section .image-column .video-link .link {
  position: relative;
  display: block;
  font-size: 22px;
  color: #191e34;
  font-weight: 400;
  text-align: center;
  height: 100px;
  width: 100px;
  line-height: 100px;
  background-color: #ffffff;
  border-radius: 50%;
  box-shadow: 0 30px 50px rgba(8, 13, 62, 0.15);
  -webkit-transition: all 300ms ease;
  -moz-transition: all 300ms ease;
  -ms-transition: all 300ms ease;
  -o-transition: all 300ms ease;
  transition: all 300ms ease;
}
</style>
