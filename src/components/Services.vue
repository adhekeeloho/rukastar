<template>
    <div class="mt-10" style="font-family: 'Poppins', sans-serif">
        <div class="font-weight-bold" style="text-align: center; font-size: 30px; margin-top: 20px; "><h4>Services</h4></div>
        <v-card class="mx-auto" max-width=" 1040">
            <div>
                <v-row dense>
                    <v-col v-for="card in cards" :key="card.title" cols="12" sm="4" ml-3>
                        <v-card>
                            <v-img :src="card.src" class="white--text align-end"
                                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)" height="400px">

                                <v-card-title v-text="card.title"></v-card-title>
                                <v-card-subtitle >This is how business are made</v-card-subtitle>
                                <v-card-subtitle class="d-flex"> <p class="mb-2 mr-3"  style="cursor: pointer"
                          @click="
                              $router.push({
                                  name: 'about',
                              })
                              ">Learn More</p> <svg-icon type="mdi" :path="path"></svg-icon></v-card-subtitle>
                            </v-img>

                        </v-card>
                    </v-col>
                </v-row>
            </div>
        </v-card>
    </div>
</template>

<script>
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiArrowRight } from '@mdi/js';

export default {
    components: {
        SvgIcon
    },
    data: () => ({
        path: mdiArrowRight,
        cards: [
            { title: 'African Foods', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 4 },
            { title: 'Natural Spices', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 4 },
            { title: 'Agro Commodities', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 4 },
        ],
    }),
}

</script>