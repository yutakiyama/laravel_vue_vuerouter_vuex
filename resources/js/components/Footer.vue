<template>
  <footer class="footer">
    <button v-if="isLogin" class="button button--link">Logout</button>
    <RouterLink v-else class="button button--link" to="/login">
      Login / Register
    </RouterLink>
  </footer>
</template>


<script>
  export default {
    computed: {
      isLogin () {
        return this.$store.getters['auth/check']
      }
    }
  }
</script>
