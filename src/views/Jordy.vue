<template>
  <div class="jordy">
    <h1>This is Jordy page</h1>
    <jordy />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Jordy from "@/components/Jordy.vue";

export default Vue.extend({
  name: "JordyView",
  components: {
    Jordy
  }
});
</script>
