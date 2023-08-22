<template>
  <div style="font-family: 'Poppins', sans-serif">
    <section id="about" class="">
      <v-row class="white great" no-gutters>
        <v-col class="pa-5 d-flex align-center" cols="12" md="5">
          <div class="help">
            <div class="twelve">
              <h1>Ruka Star International Limited</h1>
            </div>
          </div>
        </v-col>

        <v-col md="7">
          <v-img
            cover
            class="rounded"
            :src="require('../assets/African_Dishes.jpg')"
            height="600px"
          />
        </v-col>
      </v-row>
    </section>

    <section>
      <div class="ok two">
        <v-card
          max-width="900"
          class="d-flex justify-space-between"
          height="auto"
          style="
            background-color: rgb(236, 245, 242);
            font-family: 'Poppins', sans-serif;
          "
        >
          <div class="row ma-5">
            <div class="d-flex col">
              <svg-icon
                type="mdi"
                :path="food"
                style="color: #004d40; height: 50px; width: 100px"
                class="mr-2"
              ></svg-icon>
              <div>
                <h3>Natural Spices</h3>
                <p>
                  We provide natural spices such as ginger powder, garlic
                  powder, tumeric powder, suya spices, pepper soup spices etc.
                </p>
              </div>
            </div>
            <div class="d-flex col" max-width="200" color="teal lighten-5">
              <svg-icon
                style="color: #004d40; height: 50px; width: 100px"
                type="mdi"
                :path="spice"
                class="mr-2"
              ></svg-icon>
              <div>
                <h3>Natural Spices</h3>
                <p>
                  We provide natural spices such as ginger powder, garlic
                  powder, tumeric powder, suya spices, pepper soup spices etc.
                </p>
              </div>
            </div>
            <div class="d-flex col" max-width="200" color="teal lighten-5">
              <svg-icon
                type="mdi"
                :path="cocoa"
                style="color: #004d40; height: 40px; width: 100px"
                class="mr-2"
              ></svg-icon>
              <div>
                <h3>Agro Commodities</h3>
                <p>We provide Agro products such as Cashew and Cocoa etc.</p>
              </div>
            </div>
          </div>
        </v-card>
      </div>
    </section>
  </div>
</template>

<script>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiFoodVariant, mdiFoodTakeoutBox, mdiPeanut } from "@mdi/js";

export default {
  name: "Home",
  components: {
    SvgIcon,
  },
  data() {
    return {
      food: mdiFoodVariant,
      spice: mdiFoodTakeoutBox,
      cocoa: mdiPeanut,
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins&display=swap");

.ok {
  position: relative;
  bottom: 100px;
}
.help {
  margin: 60px;
}

.two {
  display: flex;
  justify-content: center;
}

.great {
  display: flex;
}

@media (min-device-width: 350px) and (max-device-width: 480px) {
  .ok {
    margin: 5px;
    position: 0;
    bottom: 0;
  }

  .help {
    margin: 5px;
    position: 0;
    top: 0x;
  }

  .great {
    display: flex;
    flex-direction: column-reverse;
  }
}

.twelve h1 {
  font-size: 26px;
  font-weight: 700;
  letter-spacing: 1px;
  text-transform: uppercase;
  width: 160px;
  text-align: center;
  margin: auto;
  white-space: nowrap;
  padding-bottom: 13px;
  font-family: "Playfair Display", serif;
}
.twelve h1:before {
  background-color: #218676;
  content: "";
  display: block;
  height: 4px;
  width: 80px;
  margin-bottom: 5px;
}
.twelve h1:after {
  background-color: #218676;
  content: "";
  display: block;
  position: relative;
  left: 450px;
  bottom: 0;
  height: 4px;
  width: 80px;
  margin-bottom: 0.25em;
}
</style>
