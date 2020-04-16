<template>
  <div class="user">
    <h2>{{ name }}</h2>
    <p>{{ bio }}</p>
  </div>
</template>
// /*eslint eol-last: ["error", "always"]*/
<script>
export default {
  name: 'User',
  props: {
    name: String,
    bio: String
  }
}
</script>
