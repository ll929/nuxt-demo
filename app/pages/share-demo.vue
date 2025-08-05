<script setup lang="ts">
import {useRoute} from "#imports";

const route = useRoute()

const url = route.query.url as string
</script>

<template>
<div>
  <template v-if="url">
    <Head>
      <Meta property="og:title" content=""/>
      <Meta property="og:description" content=""/>
      <Meta property="twitter:title" content=""/>
      <Meta property="twitter:description" content=""/>
      <Meta property="og:site_name" content=""/>
      <Meta property="og:type" content="website"/>
      <Meta property="twitter:card" content="summary_large_image"/>
      <Meta property="twitter:site" content="@Demo"/>
      <Meta property="twitter:creator" content="@Demo"/>
      <Meta property="twitter:image" :content="url"/>
      <Meta property="og:image" :content="url"/>
    </Head>
  </template>
  share demo</div>
</template>

<style scoped>

</style>