<template>
  <footer class="footer-section" style="font-family: 'Poppins', sans-serif">
    <div class="container">
      <div class="footer-content pt-5 pb-5">
        <div class="row">
          <div class="col-xl-4 col-lg-4 mb-50">
            <div class="footer-widget">
              <div class="footer-logo">
                <a href="#"
                  ><v-img
                    alt="Ruka Star"
                    class="shrink mr-2"
                    contain
                    src="../assets/logostar.png"
                    transition="scale-transition"
                    width="60"
                    height="60"
                /></a>
                
                <h5 class="mt-3" style="color: white">Ruka Star <br>International Limited</h5>
              </div>
            </div>
          </div>
          <div class="col-xl-4 col-lg-4 col-md-6 mb-30">
            <div class="footer-widget">
              <ul style="color: white">
                <li>
                  Contact Address: 12 SHEM JOSHUA STREET Opposite TRADEFAIR
                  Satellite Town Lagos
                </li>
                <li>Contact Email: rukastar@gmail.com</li>
                <li>Contact Phone: +234 816 912 4298</li>
              </ul>
            </div>
          </div>
          <div class="col-xl-4 col-lg-4 col-md-6 mb-50">
            <div class="footer-widget">
              <div class="footer-text mb-25">
                <p>
                  Privacy Policy Copyright ©
                  {{ new Date().getFullYear() }} RukaStar Limited. All rights
                  reserved
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
ul {
  margin: 0px;
  padding: 0px;
}
.footer-section {
  background: #004d40;
  position: relative;
}
.footer-content {
  position: relative;
  z-index: 2;
}
.footer-logo {
  margin-bottom: 30px;
}
.footer-logo img {
  max-width: 200px;
}
.footer-text p {
  margin-bottom: 14px;
  font-size: 14px;
  color: white;
  line-height: 28px;
}

.footer-widget ul li {
  display: inline-block;
  margin-bottom: 12px;
}
.footer-widget ul li a:hover {
  color: #ff5e14;
}
.footer-widget ul li a {
  color: #878787;
  text-transform: capitalize;
}
</style>
