<script setup lang="ts">
import {useRoute,useRequestURL} from "#imports";

const route = useRoute()

const url = route.query.url as string
const fullUrl = useRequestURL().href;
</script>

<template>
  <div>
    <template v-if="url">
      <Head>
        <Meta name="twitter:image" :content="url"/>
        <Meta property="og:image" :content="url"/>
        <Meta hid="i18n-og-url" property="og:url" :content="fullUrl"/>
      </Head>
    </template>
    share demo
  </div>
</template>

<style scoped>

</style>