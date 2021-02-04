<template>
  <div class="main">
    <h1>This is an one page</h1>
    <div class="form">
      <label for="name">Name</label>
      <input
        id="name"
        type="text"
        v-model="name"
        placeholder="João"
        maxlength="50"
      />
      <label for="name">Last Name</label>
      <input
        id="lastName"
        type="text"
        v-model="lastName"
        placeholder="Silva"
        maxlength="50"
      />
      <p v-if="name && lastName">
        Full name is {{ `${name} ${lastName}` }}.
      </p>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      name: '',
      lastName: ''
    }
  },
  mounted () {
    console.log(`in mounted ${this.name} ${this.lastName}`)
    console.log(this.$route)
  },
  unmounted () {
    console.log(`in destroyed ${this.name} ${this.lastName}`)
    console.log(this.$route)
  }

}
</script>
<style scoped>
.main {
  display: block;
}
.form {
  padding: 5px 5px;
  border-radius: 5px;
}
label {
  padding: 5px 5px;
}
</style>
