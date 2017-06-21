<template>
  <div class="Tweet">
    {{ tweet }}
  </div>
</template>

<script>
export default {
  name: 'tweet',
  props : [tweet: {auteur: 'drumpf', message: 'covfefe'}]
}
</script>

<style>
</style>
