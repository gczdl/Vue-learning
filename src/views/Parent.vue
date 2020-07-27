<template>
  <div>
    <h1>Parnet</h1>
    <m-child :msg="msg" @showMsg="showMsg" ref="child"></m-child>
  </div>
</template>

<script>
import MChild from './Child'
export default {
  data() {
    return {
      msg: '',
    }
  },
  components: { MChild },
  methods: {
    showMsg(val) {
      this.msg = val
    },
    mounted() {
      console.log(this.$children[0])
      console.log(this.$refs.child)
    },
  },
}
</script>

<style scoped></style>
