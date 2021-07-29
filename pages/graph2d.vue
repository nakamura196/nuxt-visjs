<template>
  <v-container>
    <graph2d :items="items" :options="options"> </graph2d>
  </v-container>
</template>
<script>
import { Graph2d } from 'vue-visjs'

export default {
  components: {
    graph2d: Graph2d,
  },
  data() {
    return {
      items: [
        { x: '2014-06-11', y: 10 },
        { x: '2014-06-12', y: 25 },
        { x: '2014-06-13', y: 30 },
        { x: '2014-06-14', y: 10 },
        { x: '2014-06-15', y: 15 },
        { x: '2014-06-16', y: 30 },
      ],
      options: {
        style: 'bar',
        barChart: { width: 50, align: 'center' }, // align: left, center, right
        drawPoints: false,
        dataAxis: {
          icons: true,
        },
        orientation: 'top',
        start: '2014-06-10',
        end: '2014-06-18',
      },
    }
  },
}
</script>
