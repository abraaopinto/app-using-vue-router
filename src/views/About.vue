<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="handleBack" >Back</button>
  </div>
</template>
<script>
export default {
  methods: {
    handleBack () {
      this.$router.go(-1)
    }
  }
}
</script>
