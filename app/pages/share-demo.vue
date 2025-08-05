<script setup lang="ts">
import {useRoute} from "#imports";

const route = useRoute()

const url = route.query.url as string
</script>

<template>
<div>
  <template v-if="url">
    <Head>
<!--      <Meta property="og:title" content=""/>
      <Meta property="og:description" content=""/>
      <Meta property="twitter:title" content=""/>
      <Meta property="twitter:description" content=""/>
      <Meta property="og:site_name" content=""/>
      <Meta property="og:type" content="website"/>
      <Meta property="twitter:card" content="summary_large_image"/>
      <Meta property="twitter:site" content="@Demo"/>
      <Meta property="twitter:creator" content="@Demo"/>
      <Meta property="twitter:image" :content="url"/>
      <Meta property="og:image" :content="url"/>-->

      <Meta property="og:title" content="加密衍生品交易所 | 買賣和交易加密貨幣 | Bitunix"/>
      <Meta property="og:description" content="Bitunix - 領先的加密衍生品交易所，讓您的交易更輕鬆。買入、賣出、交易 BTC 和另類貨幣，並輕鬆進入期貨市場。"/>
      <Meta name="twitter:description" content="Bitunix - 領先的加密衍生品交易所，讓您的交易更輕鬆。買入、賣出、交易 BTC 和其他代幣，並輕鬆進入期貨市場"/>
      <Meta name="keywords" content="Bitunix,Bitunix 官網,Crypto Exchange,Cryptocurrency Exchange,Bitcoin Exchange"/>
      <Meta name="description" content="Bitunix - 領先的加密貨幣衍生品交易所，輕鬆購買、出售、交易BTC等加密貨幣，並隨時隨地交易衍生品。"/>
      <Meta property="og:site_name" content="Bitunix"/>
      <Meta property="og:type" content="website"/>
      <Meta name="twitter:card" content="summary_large_image"/>
      <Meta name="twitter:site" content="@Bitunix"/>
      <Meta name="twitter:creator" content="@Bitunix"/>
      <Meta name="twitter:image" :content="url"/>
      <Meta property="og:image" :content="url"/>
    </Head>
  </template>
  share demo</div>
</template>

<style scoped>

</style>