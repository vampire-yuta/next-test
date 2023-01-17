<template>
  <h1>UserID: {{ user.name }}</h1>
</template>

<script>
export default {
  data() {
    console.log(this);
    console.log(this.$route);
    return {
      id: this.$route.params.id,
      users: [
        {
          id: 1,
          name: "John",
        },
        {
          id: 2,
          name: "Maiko",
        },
        {
          id: 3,
          name: "Yuta",
        },
      ],
    };
  },
  mounted() {
    console.log("----mounted");
    console.log(this);
  },
  created() {
    console.log("----created");
    console.log(this);
  },
  computed: {
    user() {
      return this.users.find((user) => user.id == this.id);
    },
  },
};
</script>
