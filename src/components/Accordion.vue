<template>
  <div>
    <h1>{{ item_prop.title }}</h1>
    <p @click="toggle = !toggle">
      <strong>Details</strong>
    </p>
    <p v-if="toggle">{{ item_prop.description }}</p>
    <hr />
  </div>
</template>

<script>
export default {
  name: "Accordion",

  props: ["item_prop"],

  data() {
    return {
      toggle: false,
    };
  },
};
</script>

<style scoped>

</style>