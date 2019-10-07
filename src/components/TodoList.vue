<template>
    <div>
        <h1>Kebab de Syrie</h1>
        <TodoInputText />
        <TodoListItem />
    </div>
</template>

<script>
import TodoInputText from "@/components/TodoInputText.vue";
import TodoListItem from '@/components/TodoListItem.vue';

export default  {
components: {
    TodoInputText,
    TodoListItem,
  },
  data() {
    return {
      todos: ["Salades", "Tomates", "Oignons"]
    };
  }
};

</script>

<style>

</style>