<template>
  <div>
    <h1>Weather Forecast</h1>
    {{ response }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      response: []
    }
  },
  async mounted() {
    this.response = await this.$axios.$get('weatherforecast')
  }
}
</script>
