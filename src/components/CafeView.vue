<template>
    <div>
        <v-row>
            <v-col>
                <v-breadcrumbs :items="breadcrumbs_items"></v-breadcrumbs>
            </v-col>
        </v-row>
        <v-row>
            <v-col md="5">
                <v-card>
                    <v-img
                    height="350px"
                    src="https://smarttouchpos.eu/wp-content/uploads/2018/07/75f25126bc47d2640ec06bf5a156fb86.jpg"
                    class="d-flex align-end"
                    >
                       <v-card-title>
                           <h2 class="text-h2 white--text">K-FOOD</h2>
                       </v-card-title>

                    </v-img>
                </v-card>
            </v-col>
            <v-col md="7">
                <v-card class="h-100">
                    <v-card-text>
                        <h3 class="text-h5 mb-4">Come here if you wanna to taste cool ramen</h3>
                    <v-divider></v-divider>
                    <p class="mt-4 text-body-1 mr-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel iure tempora quidem in temporibus, quos debitis alias repellat dolore aspernatur. Fuga eos possimus aperiam repudiandae aliquid nobis, soluta ut aut!</p>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
        <v-row class="cafe_menu">
            <v-col md="6">
                <v-card>
                    <v-img
                        height="450"
                        src="https://dnepr.info/wp-content/uploads/2020/05/kafe.jpg"
                        class="flex aligh-end"
                    >
                        <v-card-title>
                            <h2 class="text-h2 white--text">MENU</h2>
                        </v-card-title>

                    </v-img>
                </v-card>
            </v-col>
            <v-col md="6">
                <v-card>
                    <v-card-text>
                        <v-list-item-group>
                            <v-list-item v-for="item in menu_items" :key="item.id">
                                <v-list-item-avatar>
                                    <v-img :src="item.img">

                                    </v-img>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title class="text-subtitle-1">
                                        {{ item.title }}
                                    </v-list-item-title>
                                    <v-list-item-subtitle class="text-body-1">
                                        {{ item.price }}
                                    </v-list-item-subtitle>
                                </v-list-item-content>
                                <v-list-item-action>
                                    <v-btn icon>
                                        <v-icon color="purple lighten-1">mdi-plus</v-icon>
                                    </v-btn>

                                </v-list-item-action>
                            </v-list-item>
                        </v-list-item-group>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
    </div>
</template>

<script>
export default {
    name: 'CafeView',
    data: () => ({
        breadcrumbs_items: [
            {
                text: 'Home',
                disabled: false,
                href: '/'
            },
            {
                text: 'K-FOOD',
                disabled: true,
                href: '/cafe/view'
            }
        ],
        menu_items: [
            {
                id: 0,
                title: 'Sapporo Miso Ramen',
                img: 'https://the-challenger.ru/wp-content/uploads/2018/05/shutterstock_379968754-800x577.jpg',
                price: 35.99
            },
            {
                id: 1,
                title: 'Sapporo Miso Ramen',
                img: 'https://the-challenger.ru/wp-content/uploads/2018/05/shutterstock_379968754-800x577.jpg',
                price: 35.99
            },
            {
                id: 2,
                title: 'Sapporo Miso Ramen',
                img: 'https://the-challenger.ru/wp-content/uploads/2018/05/shutterstock_379968754-800x577.jpg',
                price: 35.99
            },
            {
                id: 3,
                title: 'Sapporo Miso Ramen',
                img: 'https://the-challenger.ru/wp-content/uploads/2018/05/shutterstock_379968754-800x577.jpg',
                price: 35.99
            }
        ]
    })
}
</script>

<style type="text/css">
    h1-100{
        height: 100%;
    }
</style>