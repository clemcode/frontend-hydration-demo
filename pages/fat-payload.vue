<script setup>
const { data } = await useFetch('https://pokeapi.co/api/v2/pokemon?offset=0&limit=1000')
const { payload } = useNuxtApp()

const bulbasaur = computed(() => data?.value?.results?.find(pokemon => pokemon.name === 'bulbasaur'))

</script>

<template>
  <div>
    <h1>Fat Payload</h1>
    <pre>
      {{ bulbasaur }}
    </pre>
  
    <ClientOnly>
      <details>
        <summary>
          Show Payload
        </summary>
        <pre>
          {{ payload }}
        </pre>
      </details>
    </ClientOnly>
  </div>
</template>