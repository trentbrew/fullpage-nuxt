# Fullpage Scroll for Nuxt 3

[Demo](https://codepen.io/tbrew1023/pen/XWymovW)

# Usage

```vue
<script setup>
const state = reactive({
  active: 0,
});

function handleScroll(e) {
  state.active = e.activeSection;
}
</script>

<template>
  <FullPage @scroll="handleScroll">
    <section id="home">Home</section>
    <section id="about">About</section>
    <section id="features">Features</section>
    <section id="showroom">Showroom</section>
    <section id="contact">Contact</section>
  </FullPage>
</template>
```
