<template>
  <div style="font-family: 'Poppins', sans-serif">
    <div
      class="d-flex justify-space-around font-weight-bold"
      style="
        text-align: center;
        font-size: 20px;
        margin-top: 20px;
        margin-bottom: 10px;
      "
    >
      <div
        style="cursor: pointer"
        @click="
          $router.push({
            name: 'home',
          })
        "
      >
        <svg-icon type="mdi" :path="path"></svg-icon>
      </div>
      <div>Agro Commodities</div>
    </div>
    <v-card class="mx-auto mb-10" max-width=" 1040">
      <div>
        <v-row>
          <v-col v-for="card in cards" :key="card.title" cols="12" sm="4">
            <v-card>
              <v-img
                :src="card.src"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="400px"
                @click.stop="dialog = true"
              >
                <v-card-title v-text="card.title"></v-card-title>
                <v-card-subtitle>This is how business are made</v-card-subtitle>
              </v-img>
            </v-card>
          </v-col>
        </v-row>
      </div>
    </v-card>
    <v-dialog v-model="dialog" max-width="290">
      <v-card>
        <v-card-title class="text-h5"> Contact Us </v-card-title>

        <v-card-text>
          <ul style="color: gray">
            <li>
              Contact Address: 12 SHEM JOSHUA STREET Opposite TRADEFAIR
              Satellite Town Lagos
            </li>
            <li>Contact Email: Linfrance@yahoo.com</li>
            <li>Contact Phone: +234 816 912 4298</li>
          </ul>
        </v-card-text>

        <v-card-actions>
          <v-spacer></v-spacer>

          <v-btn style="color: #004d40" text @click="dialog = false">
            Cancel
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>

    <section>
      <Footer/>
    </section>
  </div>
</template>

<script>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiArrowLeft } from "@mdi/js";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    SvgIcon,
    Footer,
  },
  data: () => ({
    dialog: false,
    path: mdiArrowLeft,
    cards: [
      {
        title: "Cashew",
        src: require("../assets/cashew.jpg"),
        flex: 4,
      },
      {
        title: "Bambara Seed",
        src: require("../assets/OkpaBambara.jpg"),
        flex: 4,
      },
      {
        title: "Cocoa",
        src: require("../assets/cocoa.jpg"),
        flex: 4,
      },
    ],
  }),
};
</script>
