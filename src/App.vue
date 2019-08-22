<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Curriculum Vitae</span>
        <span class="font-weight-light"> Matias Sebastian Vallarino </span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-switch
        class="mr-2 mt-6"
        v-model="$vuetify.theme.dark"
        primary
        inset 
        label="Dark"
      ></v-switch>
    </v-app-bar>

    <v-content>
      <Container/>
    </v-content>
  </v-app>
</template>

<script>
import Container from './components/Container';

export default {
  name: 'App',
  components: {
    Container,
  },
  data: () => ({
    //
  }),
};
</script>
