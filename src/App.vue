<template>
  <div>
    <input type="text" v-model="foo">
    <p>{{ bar }}</p>
  </div>
</template>
<script>
export default {
  data () {
    return {
      foo: "",
      bar: ""
    }
  },
  watch: {
    foo: function () {
      this.bar = this.foo + '!!!'
    }
  }
}
</script>
