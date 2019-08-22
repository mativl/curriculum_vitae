<template>
  <v-container>
    <v-layout
      text-center
      wrap
    >
      <v-flex mb-12 xs12>
        <Card></Card>
      </v-flex>
      <v-flex mb-12 xs12>
        <Timeline></Timeline>
      </v-flex>
      <v-flex mb-12 xs12>
        <CircularProgress :value="45"></CircularProgress>
        <CircularProgress :value="75"></CircularProgress>
        <CircularProgress :value="25"></CircularProgress>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import Card from './Card';
import Timeline from './Timeline';
import CircularProgress from './CircularProgress';

export default {
  components: {
    Card,
    Timeline,
    CircularProgress,
  }
};
</script>
