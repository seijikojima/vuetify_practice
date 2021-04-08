<template>
  <v-app>
  <v-container>
    <h1>Text and Colours</h1>

    <p class="red white--text">class="red white--text"</p>
    <p class="pink lighten-4 red--text text--darken-4">class="pink lighten-4 red--text text--darken-4"</p>

    <a href="https://vuetifyjs.com/ja/styles/colors/">color palet</a>

    <h1 class="display-4">class="display-4"</h1>
    <h1 class="display-1">class="display-1"</h1>

    <p class="headline">class="headline"</p>
    <p class="subheading font-weight-bold">class="subheading font-weight-bold"</p>
    <p class="caption">class="caption"</p>

    <h1>Button and Icons</h1>
    
    <v-btn class="pink white--text">click me</v-btn>
    <v-btn dark color="pink">click me</v-btn>
    <v-btn depressed color="pink">click me</v-btn>
    <v-btn flat color="pink">click me</v-btn>

    <v-btn depressed class="pink white--text">
      <v-icon>email</v-icon>
    </v-btn>

    <v-btn depressed class="pink white--text">
      <v-icon left small>email</v-icon>
      <span>email me</span>
    </v-btn>

    <v-btn fab depressed small dark color="purple">
      <v-icon small >favorite</v-icon>
    </v-btn>

    <a href="https://fonts.google.com/icons?selected=Material+Icons">mdi</a>

    <h1>Breakpoints and Visibility</h1>

    <v-btn class="hidden-md-and-down">class="hidden-md-and-down"</v-btn>

    <v-btn class="hidden-md-and-up">class="hidden-md-and-up"</v-btn>

    <v-btn class="hidden-sm-only">class="hidden-md-only"</v-btn>

    <h1>Theme</h1>

    <p class="success">class="success"</p>
    <p class="primary">class="primary"</p>
    <p class="warning">class="warning"</p>
    <p class="error">class="error"</p>
    <p class="info">class="info"</p>
    <p class=""></p>


  </v-container>
  </v-app>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
    })
  }
</script>
