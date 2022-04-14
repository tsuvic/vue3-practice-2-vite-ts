<template>
  <div class="home">
    <h1>Home</h1>
  </div>
  <p>
    Name in store is : {{name}}
  </p>
</template>

<script setup>
  import { computed } from 'vue'
  import { useStore } from 'vuex'

  const store = useStore()
  const name = computed(() => {
    return store.state.user.name
  })

</script>

<style>

</style>