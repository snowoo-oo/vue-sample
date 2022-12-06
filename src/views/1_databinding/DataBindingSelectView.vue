<template>
  <div>
    <select name="" id="" v-model="selectedCity">
      <option value=""></option>
      <option value="02">서울</option>
      <option value="031">경기</option>
      <option value="051">부산</option>
    </select>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      sampleData: '',
      selectedCity: '051'
    }
  }
}
</script>

<style></style>
