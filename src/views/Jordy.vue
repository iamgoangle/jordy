<template>
  <div class="jordy">
    <h1>This is Jordy page</h1>
    <jordy />
    <input-box hint="please enter your name..." />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Jordy from "@/components/Jordy.vue";
import InputBox from "@/components/InputBox.vue";

export default Vue.extend({
  name: "JordyView",
  components: {
    Jordy,
    InputBox
  }
});
</script>
