<template>
  <form>
    <div class="form-group">
      <h1>
        <slot></slot>
      </h1>
      <label>Input your name</label>
      <input type="text" class="form-control" :placeholder="hint" />
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "InputBox",
  props: {
    value: {
      type: String
    },
    hint: {
      type: String
    }
  },
  data() {
    return {
      fullname: ""
    };
  },
  methods: {
    saveName() {
      this.$emit("createName", this.fullname);
    }
  }
});
</script>