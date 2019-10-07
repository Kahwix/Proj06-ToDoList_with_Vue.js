<template>
  <div id="app">
    <TodoList />
    <TodoInputText />
  </div>
</template>

<script>
import TodoList from '@/components/TodoList.vue';
import TodoInputText from '@/components/TodoInputText.vue';

export default {
  name: "app",
  components: {
    TodoList,
    TodoInputText,
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
