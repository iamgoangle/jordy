<template>
  <div>{{ message }}</div>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "Jordy",
  data() {
    return {
      message: "Hello"
    };
  }
});
</script>
