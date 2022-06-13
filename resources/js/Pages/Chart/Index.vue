<script setup>
import BreezeAuthenticatedLayout from "@/Layouts/Authenticated.vue";
import { Head } from "@inertiajs/inertia-vue3";
</script>

<template>
  <Head title="Chart" />

  <BreezeAuthenticatedLayout>
    <template #header>
      <h2 class="font-semibold text-xl text-gray-800 leading-tight">Chart</h2>
    </template>

    <div class="py-12">
      <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
        <div class="bg-white overflow-hidden shadow-sm sm:rounded-lg">
          <div class="p-6 bg-white border-b border-gray-200">
            <BarChart class="m-20" />
            <BubbleChart class="m-20" />
            <DoughnutChart class="m-20" />
            <LineChart class="m-20" />
            <PieChart class="m-20" />
            <PolarChart class="m-20" />
            <RadarChart class="m-20" />
            <ScatterChart class="m-20" />
          </div>
        </div>
      </div>
    </div>
  </BreezeAuthenticatedLayout>
</template>

<script>
import BarChart from "@/Components/Chart/barChart.ts";
import BubbleChart from "@/Components/Chart/bubbleChart.ts";
import DoughnutChart from "@/Components/Chart/doughnutChart.ts";
import LineChart from "@/Components/Chart/lineChart.ts";
import PieChart from "@/Components/Chart/pieChart.ts";
import PolarChart from "@/Components/Chart/polarChart.ts";
import RadarChart from "@/Components/Chart/radarChart.ts";
import ScatterChart from "@/Components/Chart/scatterChart.ts";

export default {
  components: {
    BarChart,
    BubbleChart,
    DoughnutChart,
    LineChart,
    PieChart,
    PolarChart,
    RadarChart,
    ScatterChart,
  },
};
</script>