<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    <router-view> </router-view>
    {{ name }}
  </div>
</template>

<style lang="scss">
@import 'bootstrap';
</style>
<script>
export default {
  data () {
    return {
      name: process.env.VUE_APP_NAME
    }
  }
}
</script>
