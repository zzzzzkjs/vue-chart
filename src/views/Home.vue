<template>
  <div class="home">
    <Chart chart_data="" options="" />
  </div>
</template>

<script>
import Chart from "@/components/Chart.vue";

export default {
  name: "Home",
  components: {
    Chart,
  },
  data() {
    return {
      chart_data: [],
      options: [],
    };
  },
};
</script>
