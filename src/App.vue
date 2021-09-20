<template>
  <v-app>
     <Header />
    <v-main>
      <v-container>
        <div>
          <p class="text-subtitle-1 text-right">Subtitle 1</p>
          <p class="text-subtitle-2">Subtitle 2</p>
          <p class="text-body-1">Body 1</p>
          <p class="text-body-2">Body 2</p>
          <p class="text=button">Button</p>
          <p class="text-caption">Caption</p>
          <p class="text-overline">Overline</p>
          <p class="font-weight-black">Black</p>
          <p class="font-weight-bold">Bold</p>
          <p class="font-weight-medium">Medium</p>
          <p class="font-weight-regular">Regular</p>
          <p class="font-weight-light">Light</p>
          <p class="font-weight-thin">Thin</p>
        </div>
        <router-view class="view"></router-view>
      </v-container>
      
    </v-main>
    <Footer />

  </v-app>
</template>

<script>
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';


export default {
  name: 'App',

  components: {
    Header,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
