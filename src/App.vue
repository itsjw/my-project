<template>
  <div id="app">
    <div class="container">
      <div v-for="row in rows" class="columns">
          <app-card v-for="column in columns"></app-card>
      </div>
    </div>
  </div>
</template>

<script>
import Card from './components/card'

export default {
  name: 'app',
  data: function () {
    return {
      rows: 4,
      columns: 4
    }
  },
  components: {
    'appCard': Card
  }
}
</script>

<style>

</style>
