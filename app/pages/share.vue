<script setup lang="ts">
const imageUrl = ref('')
const share = (type:'x' | 'facebook') => {
  const shareUrl = window.location.origin + `/share-demo?url=${imageUrl.value}`
  switch (type){
    case "facebook":
      window.open(`http://www.facebook.com/sharer/sharer.php?u=${encodeURIComponent(shareUrl)}`,'_blank')
      return
    case "x":
      window.open(`https://twitter.com/intent/tweet?url=${shareUrl}`,'_blank')
      return;
  }
}
</script>

<template>
<div>
  <div>
    <input v-model="imageUrl"/>
  </div>
  <button @click="share('x')">share x</button>
  <button @click="share('facebook')">share Facebook</button>
</div>
</template>

<style scoped>

</style>