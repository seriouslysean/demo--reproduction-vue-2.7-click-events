<template>
  <div class="navigation-container">
    <div class="links">
      <h2>NuxtLink</h2>
      <NuxtLink to="/" @click="handleClick">Home</NuxtLink>
      <NuxtLink to="/about" @click="handleClick">About</NuxtLink>
    </div>

    <div class="links">
      <h2>NuxtLink (via BaseLink</h2>
      <BaseLink to="/" @click="handleClick">Home</BaseLink>
      <BaseLink to="/about" @click="handleClick">About</BaseLink>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    handleClick(e) {
      alert(`Target: ${e.target?.textContent}`);
    },
  },
};
</script>

<style>
.navigation-container {
  margin: 0 auto;
  min-height: 20vh;
  text-align: center;
}

.links {
  padding-top: 15px;
}
</style>
