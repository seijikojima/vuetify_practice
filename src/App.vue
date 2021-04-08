<template>
  <v-app color="grey lighten-4">

    <Navbar />
    <MainPage/>
  </v-app>
</template>

<script>
import Navbar from './components/Navbar';
import MainPage from './components/MainPage';

export default {
  name: 'App',

  components: {
    Navbar,
    MainPage,
  },

  data: () => ({
    //
  }),
};
</script>
