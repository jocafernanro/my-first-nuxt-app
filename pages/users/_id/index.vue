<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>


<script>
export default {
  validate(data) {
    return /ˆ\d+$/.test(data.params.id)
  }
};
</script>