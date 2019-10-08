<template>
  <div>
    <h1>Kebab de Syrie</h1>
    <TodoInputText v-model="newEatText" />
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
  }
};
</script>

<style>
</style>