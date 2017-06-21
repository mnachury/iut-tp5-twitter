<template>
  <div class="Timeline">
    <h1>Bienvenue sur votre timeline</h1>
    <ul>
      <li v-for="tweet in tweets">
        {{ tweet.auteur + " : " + tweet.message }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'tweets',
  data () {
    return {
      tweets: [{auteur: 'drumpf', message: 'covfefe'}, {auteur: 'petit', message: '2'}, {auteur: 'petit', message: '->'}]
    }
  }
}
</script>

<style scoped>
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: block;
    margin: 0 10px;
  }
</style>
