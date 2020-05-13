<template>
  <div id="app">
    <button @click="click">{{ state.count }}</button>
  </div>
</template>

<script>
import { reactive, computed } from 'vue'

export default {
  setup() {
    const state = reactive({
      count: 0
    });
    function click() {
      state.count += 1;
    }
    return {
      state,
      click
    }
  }
}
</script>

<style>

</style>
