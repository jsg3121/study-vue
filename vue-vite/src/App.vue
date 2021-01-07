<template>
  <div>
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Hello Vue 3.0 + Vite" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import mix from './mixins/mix'

export default {
  name: 'App',
  mixins: [mix],
  components: {
    HelloWorld
  },
  created() {
    this.mixTest();
  },
  methods: {
    mixTest() {
      this.testing();
    }
  }
}
</script>
