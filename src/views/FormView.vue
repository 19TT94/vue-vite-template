<script setup lang="ts">
import Form from "@/components/Form.vue";
</script>

<template>
  <main class="form-view">
    <section class="form">
      <Form />
    </section>
  </main>
</template>

<style lang="scss">
@import "@/assets/style/all.scss";

.form-view {
  position: relative;
  width: 100%;
}

.form {
  width: 100%;
  background: $gray;
  max-width: $bp-4;
  margin: 0 auto;
  padding: $pad;
}

.title {
  font-style: italic;
  margin-top: $pad * 3;

  @include bp(2) {
    margin-top: 0;
  }
}
</style>
