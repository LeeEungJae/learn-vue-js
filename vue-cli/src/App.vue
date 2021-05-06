<template>
  <div class="app">
    <app-header v-bind:propsdata="str" v-on:renew="renewString" />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
export default {
  data() {
    return {
      str: "Header",
    };
  },
  components: {
    AppHeader,
  },
  methods: {
    renewString: function() {
      this.str = "hi";
    },
  },
};
</script>

<style></style>
