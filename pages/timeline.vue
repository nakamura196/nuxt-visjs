<template>
  <v-container>
    <timeline ref="timeline" :items="items" :groups="groups" :options="options">
    </timeline>
  </v-container>
</template>
<script>
import { Timeline } from 'vue-visjs'

export default {
  components: {
    timeline: Timeline,
  },
  data() {
    return {
      groups: [
        {
          id: 0,
          content: 'Group 1',
        },
      ],
      items: [
        {
          id: 0,
          group: 0,
          start: new Date(),
          content: 'Item 1',
        },
      ],
      options: {},
    }
  },
}
</script>
