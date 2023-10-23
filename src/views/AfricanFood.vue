<template>
    <div style="font-family: 'Poppins', sans-serif">
        <div class="d-flex justify-space-around font-weight-bold" style="text-align: center; font-size: 20px; margin-top: 20px; margin-bottom: 10px;" >
            <div style="cursor: pointer"
                        @click="
                            $router.push({
                                name: 'home',
                            })
                            "
                               ><svg-icon type="mdi" :path="path"></svg-icon></div>
            <div >African Foods</div>
        </div>
        <v-card class="mx-auto mb-10" max-width=" 1040">
            <div>
                <v-row>
                    <v-col v-for="card in cards" :key="card.title" cols="12" sm="4">
                            <v-card>
                                <v-img :src="card.src" class="white--text align-end"
                                    gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)" height="400px" @click.stop="dialog = true">

                                    <v-card-title v-text="card.title"></v-card-title>
                                    <v-card-subtitle >This is how business are made</v-card-subtitle>
                                   
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
          <Footer />
        </section>
    </div>
</template>

<script>
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiArrowLeft } from '@mdi/js';
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
            { title: 'Palm Oil', src: require("../assets/PalmOil.jpg"), flex: 4 },
            { title: 'Garri', src: require("../assets/IjebuGarri.jpg"), flex: 4 },
            { title: 'Abacha(cassava flakes)', src: require("../assets/Tapioca.jpg"), flex: 4 },
            { title: 'Melon', src: require("../assets/Egusi.jpg"), flex: 4 },
            { title: 'Ogbono', src: require("../assets/Ogbono.jpg"), flex: 4 },
            { title: 'Honey Beans', src: require("../assets/HoneyBeans.jpg"), flex: 4 },
            { title: 'Kuli Kuli(peanut bars)', src: require("../assets/kulikuli.jpg"), flex: 4 },
            { title: 'Groundnut Oil(kuli kuli oil only)', src: require("../assets/AllFood.jpg"), flex: 4 },
            { title: 'Cocoyam Flour', src: require("../assets/yamflour.jpg"), flex: 4 },
            { title: 'Dried Ukwa', src: require("../assets/DriedUkwa.jpg"), flex: 4 },
            { title: 'Bambara/Okpa Flour', src: require("../assets/OkpaBambara.jpg"), flex: 4 },
            { title: 'Fufu Flour', src: require("../assets/AllFood.jpg"), flex: 4 },
            { title: 'Yam Flour', src: require("../assets/yamflour.jpg"), flex: 4 },
            { title: 'Fish', src: require("../assets/Fish.jpg"), flex: 4  },
             { title: 'Cray Fish ', src: require("../assets/crayfish.jpg"), flex: 4 },
        ],
    }),
}
</script>