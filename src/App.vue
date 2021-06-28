<template>
  <h1 class="text-3xl" style="color: red">
    This text should be green in dark mode!
  </h1>
  <h2 class="text-3xl" style="color: red">This text is green in dark mode!</h2>
</template>

<style lang="postcss">
h1 {
  @apply dark:!text-green-500;
}
@media (prefers-color-scheme: dark) {
  h2 {
    @apply !text-green-500;
  }
}
</style>
