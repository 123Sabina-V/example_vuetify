<template>
<v-row>
    <v-col class="cafe_component">
        <h1 class="py-4">Lists of cafes</h1>

        <v-row class="cafe_list mx-2">
            <v-col v-for="cafe in cafes" :key="cafe.id" md="4">
                <v-card class="cafe_card">
                    <v-img
                        height="250"
                        :src="cafe.img"
                    ></v-img>  
                    <v-card-title>
                        <router-link to="/cafe/view">{{ cafe.name }}
                        </router-link>
                    </v-card-title>
                    <v-card-text>
                        <p>{{ cafe.description }}</p>
                        <b>Rating: {{ cafe.rating }} of 5</b>
                    </v-card-text>
                </v-card>
            </v-col>

        </v-row>
    </v-col>
</v-row>
</template>

<script>
    export default {
        name: 'Cafe',
        data: () => ({
            cafes: [
                {
                    id: 0,
                    name: 'K-FOOD',
                    description: 'Here we can cook nice korean food',
                    img: 'http://c.files.bbci.co.uk/9017/production/_105278863_gettyimages-855098134.jpg',
                    tags: ['asian'],
                    rating: 5
                },
                {
                    id: 1,
                    name: 'K-FOOD',
                    description: 'Here we can cook nice korean food',
                    img: 'http://c.files.bbci.co.uk/9017/production/_105278863_gettyimages-855098134.jpg',
                    tags: ['asian'],
                    rating: 5
                },
                {
                    id: 2,
                    name: 'K-FOOD',
                    description: 'Here we can cook nice korean food',
                    img: 'http://c.files.bbci.co.uk/9017/production/_105278863_gettyimages-855098134.jpg',
                    tags: ['asian'],
                    rating: 5
                },
                {
                    id: 3,
                    name: 'K-FOOD',
                    description: 'Here we can cook nice korean food',
                    img: 'http://c.files.bbci.co.uk/9017/production/_105278863_gettyimages-855098134.jpg',
                    tags: ['asian'],
                    rating: 5
                },
                {
                    id: 4,
                    name: 'K-FOOD',
                    description: 'Here we can cook nice korean food',
                    img: 'http://c.files.bbci.co.uk/9017/production/_105278863_gettyimages-855098134.jpg',
                    tags: ['asian'],
                    rating: 5
                },
                 {
                    id: 5,
                    name: 'K-FOOD',
                    description: 'Here we can cook nice korean food',
                    img: 'http://c.files.bbci.co.uk/9017/production/_105278863_gettyimages-855098134.jpg',
                    tags: ['asian'],
                    rating: 5
                }
            ]
    })
    }
</script>
