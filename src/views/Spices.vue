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
                <div >Natural Spices</div>
            </div>
        <v-card class="mx-auto" max-width=" 1040">
            <div>
                <v-row>
                    <v-col v-for="card in cards" :key="card.title" cols="12" sm="4">
                        <v-card>
                            <v-img :src="card.src" class="white--text align-end"
                                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)" height="400px">

                                <v-card-title v-text="card.title"></v-card-title>
                                <v-card-subtitle>This is how business are made</v-card-subtitle>

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
import { mdiArrowLeft } from '@mdi/js';

export default {
    components: {
        SvgIcon
    },
    data: () => ({
        path: mdiArrowLeft,
        cards: [
            { title: 'African Foods', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 4 },
            { title: 'Natural Spices', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 4 },
            { title: 'Agro Commodities', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 4 },
            { title: 'African Foods', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 4 },
            { title: 'Natural Spices', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 4 },
            { title: 'Agro Commodities', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 4 },
            { title: 'African Foods', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 4 },
            { title: 'Natural Spices', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 4 },
            { title: 'Agro Commodities', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 4 },
        ],
    }),
}
</script>