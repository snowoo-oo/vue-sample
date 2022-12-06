<template>
  <div>
    <div>
      <input type="radio" id="html" value="HTML" v-model="selectInput" />
      <label for="html">HTML</label>
    </div>
    <div>
      <input type="radio" id="css" value="CSS" v-model="selectInput" />
      <label for="css">CSS</label>
    </div>
    <div>
      <input type="radio" id="js" value="JS" v-model="selectInput" />
      <label for="js">JS</label>
    </div>
    <div>selected : {{ selectInput }}</div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      selectInput: 'nothing'
    }
  }
}
</script>

<style></style>
