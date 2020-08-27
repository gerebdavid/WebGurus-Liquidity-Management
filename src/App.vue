<template>
  <v-app>

    <v-app-bar
      app
      color="blue-grey lighten-1"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="WebGurus"
          class="shrink mr-2"
          contain
          src="https://www.webgurus.biz/wp-content/uploads/2018/03/logo_webgurus@2x.png"
          transition="scale-transition"
          width="40"
          href="https://www.webgurus.biz"
        />
      </div>
    </v-app-bar>

    <v-main>
      <FormPage/>
      <!-- <LoginPage/> -->

    </v-main>
  </v-app>

  
</template>

<script>
//import LoginPage from './components/LoginPage';
import FormPage from './components/FormPage';

export default {
  name: 'App',

  components: {
    //LoginPage,
    FormPage,
  },

  data: () => ({
    //
  }),
};
</script>
