<script setup lang="ts">
import {useRoute} from "#imports";

const route = useRoute()

const url = route.query.url as string
</script>

<template>
  <div>
    <template v-if="url">
      <Head>
        <Meta name="twitter:image" :content="url"/>
        <Meta property="og:image" :content="url"/>
      </Head>
    </template>
    share demo
  </div>
</template>

<style scoped>

</style>