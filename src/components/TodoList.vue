<template>
  <div>
    <h1>Kebab de Syrie</h1>
    <TodoInputText v-model="newEatText" @keydown.enter="addTodo" />
    <TodoListItem :bouf="bouf" />
  </div>
</template>

<script>
import TodoInputText from "@/components/TodoInputText.vue";
import TodoListItem from "@/components/TodoListItem.vue";

export default {
  components: {
    TodoInputText,
    TodoListItem
  },
  data() {
    return {
      newEatText: "eat",
      bouf: ["Salades", "Tomates", "Oignons"]
    };
  },
  methods: {
    addTodo() {
      const trimmedText = this.newTodoText.trim();
      if (trimmedText) {
        this.todos.push(trimmedText);
        this.newTodoText = "";
      }
    }
  }
};
</script>

<style>
</style>