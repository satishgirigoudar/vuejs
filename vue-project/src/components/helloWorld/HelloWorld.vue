<template>
  <h1>hello {{ name }}</h1>
  <h2 v-text="name"></h2>
</template>

<script>
export default {
  data() {
    return {
      name : 'satish'
    }
  }
}
</script>