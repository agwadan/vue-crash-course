<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="AddTask" color="green" />
  </header>
</template>

<script>
import Button from "./Button.vue";
export default {
  name: "Header",
  props: {
    title: String,
  },
  components: {
    Button,
  },
};
</script>

<style scoped>
/* Scoped means this styling applies only to this component */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
