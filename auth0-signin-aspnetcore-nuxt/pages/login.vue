<template>
  <div>
    <h1>Login</h1>
    <button @click="onClick">Login with Auth0</button>
  </div>
</template>

<script>
export default {
  methods: {
    onClick() {
      this.$auth.loginWith('auth0')
    }
  }
}
</script>
