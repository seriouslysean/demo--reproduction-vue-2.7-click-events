<template>
  <NuxtLink v-bind="$attrs">
    <span v-on="$listeners">
      <slot />
    </span>
  </NuxtLink>
</template>

<script>
export default {
  name: 'BaseLink',
  inheritAttrs: false,
};
</script>
