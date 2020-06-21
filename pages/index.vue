<template>
  <div class="container">
    <a href="/users">Users with href</a>
    <nuxt-link to="/users">Users with Nuxt link</nuxt-link>
    <button @click="onLoadProducts">Go to products</button>
  </div>
</template>

<script>
export default {
  components: {
  },
  methods: {
    onLoadProducts() {
      this.$router.push('/products')
    }
  }
}
</script>

<style>

</style>
