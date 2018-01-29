<template>
  <div>
    <h3>新的記事</h3>
    <button @click="counter++">新增</button>
    <p>{{ counter }}</p>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        counter: 0
      }
    },
    destroyed() {
      console.log('destroyed')
    },
    deactivated() {
      console.log('Deactivated')
    },
    activated() {
      console.log('Activated')
    }
  }
</script>