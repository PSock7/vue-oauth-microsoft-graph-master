<template>
  <header class="base-header">
    <div class="header-content">
      <base-button>
        <font-awesome-icon class="icon" :icon="['fas', 'home']" /> Home
      </base-button>
      <base-button>
        <font-awesome-icon class="icon" :icon="['fas', 'address-book']" /> Home
      </base-button>

      <div class="separator" />

      <base-button>
        <font-awesome-icon class="icon" :icon="['fas', 'address-card']" /> About us 
      </base-button>
      <base-button>
        <font-awesome-icon class="icon" :icon="['fas', 'user']" /> Not yet logged in
      </base-button>
    </div>
  </header>
</template>

<script>
import BaseButton from './BaseButton.vue'
export default {
  name: 'BaseHeader',
  components: { BaseButton }
}
</script>

<style scoped>
.base-header {
  background-color: #42b983;
  padding: 1em;
}

.header-content {
  display: flex;
  max-width: 70em;
  margin: auto;
}

.separator {
  flex-grow: 1;
}

.icon {
  margin-right: 0.5em;
}
</style>
