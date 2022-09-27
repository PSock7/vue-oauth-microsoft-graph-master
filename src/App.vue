<template>
  <base-layout>
    <home-page />
  </base-layout>
</template>

<script>
import BaseLayout from './components/BaseLayout.vue'
import HomePage from './pages/HomePage.vue'

export default {
  name: 'App',
  components: {HomePage, BaseLayout}
}
</script>

<!-- This is a global style, since we select 'body' tag. -->
<!-- Other components should use scoped styles. -->
<style>
body {
  font-family: 'Roboto', sans-serif;
  margin: 0;
}
</style>