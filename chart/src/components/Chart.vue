<template>
  <highcharts class="hc" :options="chartOptions" ref="chart"/>
</template>

<script>
export default {
name: "Chart",
  components: {},
  data() {
  return {
    chartOptions:{
      series: [
        {
          data: [1, 2, 3]
        }
      ]
    }
  }
  }
}
</script>

<style scoped>

</style>