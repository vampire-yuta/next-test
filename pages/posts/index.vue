<template>
  <div>
    <h1>記事一覧</h1>
    <ul>
      <li v-for="post in posts" :key="post.id">
        {{ post.title }}
      </li>
    </ul>
    {{ posts }}
  </div>
</template>

<script>
export default {
  /* async asyncData({ $axios }) { */
  /*   console.log("before"); */
  /*   const posts = await $axios.$get( */
  /*     "https://jsonplaceholder.typicode.com/posts/" */
  /*   ); */
  /*   return { posts }; */
  /* }, */
  /* data() { */
  /*   return { */
  /*     posts: [], */
  /*   }; */
  /* }, */
  /* async fetch() { */
  /*   const posts = await this.$axios.$get( */
  /*     "https://jsonplaceholder.typicode.com/posts/" */
  /*   ); */
  /*   this.posts = posts; */
  /* }, */
  /* fetchOnServer: false, */

  async asyncData() {
    console.log("before");
    const posts = [
      { id: 1, title: "aaa", description: "bbb" },
      { id: 2, title: "ccc", description: "ddd" },
    ];
    return { posts };
  },
};
</script>
