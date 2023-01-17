<template>
  <div>
    <h1>About page</h1>
    <h2>{{ subtitle }}</h2>
  </div>
</template>

<script>
export default {
  layout: "original",
  data() {
    return {
      subtitle: "nuxt.js testing",
    };
  },
};
</script>
