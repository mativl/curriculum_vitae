<template>
  <v-timeline :dense="$vuetify.breakpoint.smAndDown">
    <v-timeline-item
      v-for="(item, i) in items"
      :key="i"
      :color="item.color"
      :icon="item.icon"
      fill-dot
    >
      <template v-slot:opposite>
        <span
          :class="`headline font-weight-bold ${item.color}--text`"
          v-text="item.year"
        ></span>
      </template>
      <v-card
        :color="item.color"
        dark
      >
        <v-card-title class="title">{{item.title}}</v-card-title>
        <v-card-text class="white text--primary">
          <p>{{item.text}}</p>
          <v-btn
            :color="item.color"
            class="mx-0"
            outlined
          >
            Button
          </v-btn>
        </v-card-text>
      </v-card>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
export default {
  data: () => ({
      items: [
        {
          color: 'cyan',
          icon: 'mdi-star',
          year: '2010',
          title: 'titulo1',
          text: 'Lorem1 ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae',
        },
        {
          color: 'green',
          icon: 'mdi-book-variant',
          year: '2011',
          title: 'titulo2',
          text: 'Lorem2 ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae',
        },
        {
          color: 'pink',
          icon: 'mdi-airballoon',
          year: '2012',
          title: 'titulo3',
          text: 'Lorem4 ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae',
        },
        {
          color: 'amber',
          icon: 'mdi-buffer',
          year: '2015',
          title: 'titulo4',
          text: 'Lorem4 ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae',
        },
      ],
    }),
}
</script>

<style>

</style>