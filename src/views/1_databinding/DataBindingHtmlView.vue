<template>
  <div>
    <h3>{{ htmlString }}</h3>
    <h3 v-html="htmlString"></h3>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      htmlString: '<p style="color:red;">빨간색</p>'
    }
  }
}
</script>

<style></style>
