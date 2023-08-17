<template>
  <div class="container">
    <section id="about" class="overflow-hidden">
      <v-row class="white" no-gutters>
        <v-col class="pa-5" cols="12" md="5">
          <!-- <h1 class="do  mt-5" style="font-family: 'Poppins', sans-serif">Who We Are</h1>
              <p class="mb-5" style="font-family: 'Poppins', sans-serif">
                Serving up a simply straightforward (and straight-up savory) pizza menus of Northern Italian classics like spicey pizza, sussage Pizza, chicken pizza, beef pizza, etc.
              </p>
              <p class="mb-5" style="font-family: 'Poppins', sans-serif">
                 We are known as a world class pizza Heaven from the inception of service to the fulfilling tastes. The Foodology is a love letter to Italy woven from a different cloth. 
              </p> -->
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

    <div class="ok two">
      <v-card class="d-flex CardHead justify-space-between" height="auto" color="teal lighten-5">
        <div class="row ma-5">
          <div class="d-flex col " color="teal lighten-5"
  >
            <svg-icon
              type="mdi"
              :path="food"
              style="color: #004d40; height: 50px; width: 100px"
              class="mr-2"
            ></svg-icon>
            <div>
              <h3>Natural Spices</h3>
              <p>
                We provide natural spices such as ginger powder, garlic powder,
                tumeric powder, suya spices, pepper soup spices etc.
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
              We provide natural spices such as ginger powder, garlic powder,
              tumeric powder, suya spices, pepper soup spices etc.
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

.two {
  display: flex;
  justify-content: center;
}

@media (min-device-width: 350px) and (max-device-width: 480px) {
  .ok {
    margin: 5px;
    position: 0;
    bottom: 0;
  }
  .CardHead {
    width: 100%;
  }
}

.CardHead {
  width: 70%;
}
</style>
