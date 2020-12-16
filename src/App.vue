<template>
  <div id="app">
    <cabecera> </cabecera>
    <pie> </pie>
  </div>
</template>

<script>

import cabecera from "./components/header.vue";
import pie from "./components/footer.vue";

export default {
  name: "App",
  components: {
    cabecera,
    pie,
  },
};
</script>

