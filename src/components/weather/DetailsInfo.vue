<template>
  <p class="font-weight-regular text-h5">
    {{ info | createText }}
  </p>
</template>

<script>
import lodash from "lodash";

export default {
  name: "DetailsInfo",
  props: ["info"],
  filters: {
    createText: function(value) {
      return `Feels like ${Math.round(value.feels)}°C.
              ${lodash.upperFirst(value.description)}`;
    }
  }
};
</script>

<style scoped></style>
