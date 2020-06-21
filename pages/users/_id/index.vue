<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>


<script>
export default {
  validate({ params, query, store }) {
    // Must be a number
    return /^\d+$/.test(params.id)
  },
  layout: 'users'
};
</script>
