<template>
  <div>
    <button @click="emitEventOne">Event 1</button>
    <button @click="emitEventTwo">Event 2</button>
    <button @click="emitEventThree">Event 3</button>
  </div>
</template>

<script>
export default {
  methods: {
    emitEventOne() {
      this.$emit('event-one')
    },
    emitEventTwo() {
      this.$emit('event-two', 'This is an argument')
    },
    emitEventThree() {
      this.$emit('event-three', 123, { name: 'three' })
    }
  }
}
</script>

<style></style>
