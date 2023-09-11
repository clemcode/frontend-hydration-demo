<script setup>
import { formatRelative, subDays } from 'date-fns'
import { es, fr } from 'date-fns/locale/index.js'

const date = formatRelative(subDays(new Date(), 3), new Date())

const esDate = formatRelative(subDays(new Date(), 3), new Date(), { locale: es })

const frDate = formatRelative(subDays(new Date(), 3), new Date(), { locale: fr })
</script>

<template>
<div>
  <p>{{ date }}</p>
  <p>{{ esDate }}</p>
  <p>{{ frDate }}</p>
</div>
</template>