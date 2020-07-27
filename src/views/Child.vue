<template>
  <div>
    <h3>child</h3>
    <h5>{{ msg }}</h5>
    <button @click="passMsg">走你</button>
  </div>
</template>

<script>
export default {
  props: {
    msg: {
      type: String,
      default: '',
    },
  },
  methods: {
    passMsg() {
      this.$emit('showMsg', 'i am from child')
    },
  },
}
</script>

<style scoped></style>
