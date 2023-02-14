<script setup>
  defineProps({
    data: {
      type: Object,
      required: true,
    },
  });
</script>

<template>
  <div class="tab-content overflow-text">
    <section>
      <h1>Content</h1>
      <pre><code v-text="data.response" /></pre>
    </section>
  </div>
</template>

<style
  lang="scss"
  scoped
>
  .error {
    padding: 1rem;
    background-color: var(--color-error);
    color: var(--color-error-text);
    border-radius: 5px;
  }
</style>
