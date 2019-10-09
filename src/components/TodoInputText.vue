<template>
  <div class="control">
    <input
      class="input is-focused"
      type="text"
      placeholder="Entrer votre Aliment"
      :value="value"
      v-on="listeners"
    />
  </div>
</template>

<script>
export default {
  props: ["value"],
  computed: {
    listeners() {
      return {
        // Pass all component listeners directly to input
        ...this.$listeners,
        // Override input listener to work with v-model
        input: event => this.$emit("input", event.target.value)
      };
    }
  }
};
</script>

<style>
</style>