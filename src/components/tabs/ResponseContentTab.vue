<script setup>
  defineProps({
    data: {
      type: Object,
      required: true,
    },
  });
</script>

<template>
  <div
    class="tab-content overflow-text"
  >
    <section>
      <h1>Content</h1>
      <pre><code v-text="JSON.stringify(data, null, 2)" /></pre>
    </section>
  </div>
</template>

<style
  lang="scss"
  scoped
>
  summary {
    margin-bottom: .3rem;
  }

  pre {
    margin: 0;
    overflow: auto;
  }

  code {
    font-family: monospace;
  }
</style>
