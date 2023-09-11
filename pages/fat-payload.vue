<template>
  <h1>Fat Payload</h1>
  <pre>
    {{ bulbasaur }}
  </pre>
</template>

<script setup>
const { data } = useFetch('https://pokeapi.co/api/v2/pokemon?offset=0&limit=1000')

const bulbasaur = computed(() => data.value?.results[0])
</script>