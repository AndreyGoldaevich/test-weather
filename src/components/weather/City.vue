<template>
  <h2 class="text-h4 font-weight-light d-block mb-6">
    {{ name }}
  </h2>
</template>

<script>
export default {
  name: "City",
  props: ["name", "id"]
};
</script>

<style scoped></style>
