<template>
  <div class="Chart">
    <h1>chart.js test page</h1>
  </div>
</template>

<script>
import { LineChart } from "vue-chartjs";

export default {
  extends: LineChart,
  name: "Chart",
  props: {
     chart_data: {
      type: Array,
      default: [],
    },
    options: {
      type: Array,
      default: [],
    },
  },
  mounted() {
    this.renderChart(this.chart_data, this.options);
  },
};
</script>

<style scoped lang="scss"></style>
