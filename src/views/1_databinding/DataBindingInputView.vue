<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="onClick">click</button>
    <button @click="changeData">click2</button>
    <br />
    <input type="text" v-model="num1" />+ <input type="text" v-model="num2" />=
    <span>{{ num1 + num2 }}</span>
    <br />
    <input type="text" v-model.number="num3" />+
    <input type="text" v-model.number="num4" />=
    <span>{{ num3 + num4 }}</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: 'test',
      num1: 1,
      num2: 2,
      num3: 3,
      num4: 4
    }
  },
  methods: {
    onClick() {
      console.log(this.userId)
    },
    changeData() {
      this.userId = 'J.WOO'
    }
  }
}
</script>

<style></style>
