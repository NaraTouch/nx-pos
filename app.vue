<template>
  <div>
    <NuxtPage/>
  </div>
</template>
<script>
import { defineNuxtPlugin } from '#app'

export default defineNuxtPlugin(nuxtApp => {
  nuxtApp.provide('injected', () => 'my injected function')
  // now available on `nuxtApp.$injected`
})
</script>
