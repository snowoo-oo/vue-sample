<template>
  <div class="databindingstring">
    <h1>Hello {{ userName }}</h1>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: 'J.Woo',
      message: 'Hello World databinding',
      arr: [],
      obj: {}
    }
  }
}
</script>

<style scoped></style>
