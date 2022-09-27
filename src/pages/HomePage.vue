<template>
  <div style="text-align: center">
    <p>Here comes the content of the HomePage.</p>

    <async-button @click="wait2Seconds">
      Disabled and animated for 2 seconds if clicked
    </async-button>
    <async-button @click="wait2SEC">Base Button</async-button>
  </div>
</template>

<script>
import AsyncButton from '../components/AsyncButton.vue'

export default {
  name: 'HomePage',
  components: { AsyncButton },
  methods: {
    wait2Seconds () {
      return new Promise(resolve => setTimeout(resolve, 2000))
    }
  }
}
</script>
