<template>
  <v-container>
    <div class="d-flex align-center justify-space-between">
      <h1 class="text-h1 mt-12 mb-12">{{ title }}</h1>
    </div>
    <AllCitiesList />
    <AddLocation />
  </v-container>
</template>

<script>
import AllCitiesList from "./AllCitiesList.vue";
import AddLocation from "./AddLocation.vue";
export default {
  data: function() {
    return {
      title: "Settings"
    };
  },
  components: {
    AllCitiesList,
    AddLocation
  },
  name: "SettingsContainer",
  props: {}
};
</script>

<style scoped></style>
