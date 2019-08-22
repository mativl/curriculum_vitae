<template>
  <v-progress-circular
    :rotate="-90"
    :size="100"
    :width="15"
    :value="init"
    color="primary"
  >{{ init }}</v-progress-circular>
</template>

<script>
export default {
  props:{
    value: Number
  },
  data () {
    return {
      interval: {},
      init: 0,
    }
  },
  beforeDestroy () {
    clearInterval(this.interval)
  },
  mounted () {
    this.interval = setInterval(() => {
      this.init += 1;
      if (this.init >= this.value) {
        clearInterval(this.interval)
      }
    }, 10);
  }
}
</script>

<style>
  .v-progress-circular {
    margin: 1rem;
  }
</style>