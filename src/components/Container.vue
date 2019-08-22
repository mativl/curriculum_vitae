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
    </v-layout>
  </v-container>
</template>

<script>
import Card from './Card';
import Timeline from './Timeline';

export default {
  components: {
    Card,
    Timeline,
  }
};
</script>
