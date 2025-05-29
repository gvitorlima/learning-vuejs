<template>
  <button @click="testeApenas()" :style="{ background: color, color: fontColor }">
    {{ text }}
  </button>
</template>

<style scoped>
button {
  background-color: #1d4ed8; /* azul mais suave */
  color: white;
  padding: 0.5rem 1rem;
  border: none;
  border-radius: 0.375rem;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.2s ease-in-out;
}
</style>

<script>
export default {
  name: 'BonitaButton',
  props: {
    text: {
      type: String,
      default: 'BonitaButton',
    },
    color: {
      type: String,
    },
    fontColor: {
      type: String,
      default: 'White',
    },
  },
  methods: {
    testeApenas() {
      console.log('Clica baixo nengue !')
    },
  },
}
</script>
