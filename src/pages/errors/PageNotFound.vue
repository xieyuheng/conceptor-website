<script setup lang="ts">
import { Head } from '@vueuse/head'
import { useRoute } from 'vue-router'

const route = useRoute()
</script>

<template>
  <div>
    <Head>
      <title>404 | Conceptor</title>
    </Head>

    <div class="flex flex-col space-y-2 p-3">
      <div class="text-3xl">404</div>

      <div>
        Page Not Found
      </div>

      <div class="overflow-x-auto">{{ route.fullPath }}</div>
    </div>
  </div>
</template>
