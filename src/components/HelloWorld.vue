<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
    <p>
      Затирка керамогранита, эпоксидная затирка кафельнной плитки.
      <code>Эпоксидная затирка керамогранита.</code> Часный мастер без посредников.
    </p>
  </div>

  <p>
   Прайс:
    <a href="/" target="_blank"
      >Цены</a
    >, Цены на укладку керамогранита и керамической плитки.
  </p>
  <p>
    Портфолио:
    <a href="/" target="_blank">Портфолио фото работ.</a>
    Укадка курамогранита по диоганали.
  </p>
  <p class="read-the-docs">Укладка кафельной плитки.</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
