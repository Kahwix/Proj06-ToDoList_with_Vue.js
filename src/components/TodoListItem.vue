<template>
  <ul>
    <li v-for="eat in bouf">{{ eat }}</li>
  </ul>
</template>

<script>
export default {
    props: ["bouf"]
}
</script>

<style>

</style>