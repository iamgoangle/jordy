<template>
  <div class="jordy">
    <h1>This is Jordy page</h1>
    <h1>Hello, {{ fullname }}</h1>
    <input-box hint="please enter your name..." @createName="setName" />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
// import Jordy from "@/components/Jordy.vue";
import InputBox from "@/components/InputBox.vue";

export default Vue.extend({
  name: "JordyView",
  data() {
    return {
      fullname: ""
    };
  },
  methods: {
    setName(name: string) {
      this.fullname = name;
    }
  },
  components: {
    // Jordy,
    InputBox
  }
});
</script>
