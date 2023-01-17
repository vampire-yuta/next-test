<template>
  <div>
    <nav>
      <p>This is navigation bar.</p>
      <nuxt-link to="/">Home</nuxt-link>
      <nuxt-link to="/about" no-prefetch>About page not prefetched</nuxt-link>
      <nuxt-link to="/about" :prefetch="false">About page not prefetched</nuxt-link>
      <nuxt-link :to="{ name: 'users-list' }">User List</nuxt-link>
    </nav>
  </div>
</template>
