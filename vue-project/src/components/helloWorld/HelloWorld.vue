<template>
  <h2>hello {{ name }}</h2>
  <h2 v-text="name"></h2>
  <h2 v-html="lastName"></h2>
  <h2 v-html="hack"></h2>
  <h2 v-bind:id="heading">Heading</h2>
  <button v-bind="{ disabled : isDisabled }" @click="showAlert">click me</button>
</template>

<script>
export default {
  data() {
    return {
      name : 'satish',
      lastName : '<b>Girigoudar</b>',
      hack : `<a href="#" onclick="alert('you have hacked')">win price pool</a>`,
      heading : 'Heading',
      isDisabled : false,
    }
  },
  methods: {
    showAlert() {
      alert('you clicked button');
    }
  }
}
</script>