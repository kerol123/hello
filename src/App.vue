<template>
  <el-container>
    <el-header>Vue Chrome Extension</el-header>
    <el-main>
      <el-button type="primary" @click="handleClick">Click Me!</el-button>
      <p>{{ message }}</p>
    </el-main>
  </el-container>
</template>

<script>
import { ref } from 'vue';

export default {
  setup() {
    const message = ref('Hello from Chrome Extension!');

    const handleClick = () => {
      message.value = 'Button Clicked!';
    };

    return { message, handleClick };
  }
};
</script>

<style>
body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 0;
}
</style>
