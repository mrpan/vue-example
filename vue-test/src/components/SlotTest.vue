<template>
<div>
  <header>
    <slot name="header"></slot>
  </header>
  <main>
    <slot name="test1"></slot>
  </main>
  <footer>
    <slot name="footer"></slot>
  </footer>
  <a v-bind:href="url" class="nav-link">
    <slot name="test2">this is slot</slot>
  </a>
</div>
</template>

<script>
export default {
  name: "SlotTest",
  props: {
    url: String,
  },
};
</script>
