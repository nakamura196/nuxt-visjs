<template>
  <v-container>
    <ul>
      <li v-for="(item, key) in items" :key="key">
        <nuxt-link :to="{ name: item.name }">{{ item.label }}</nuxt-link>
      </li>
    </ul>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          label: 'Timeline',
          name: 'timeline',
        },
        {
          label: 'Network',
          name: 'network',
        },
        {
          label: 'Graph2d',
          name: 'graph2d',
        },
      ],
    }
  },
}
</script>
