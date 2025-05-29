<template>
  <header>
    <h1>Im the Header, Mue-he he he. {{ title }}</h1>
    <BonitaButton color="#008080" text="Teal" />
    <BonitaButton color="#7FFFD4" text="Aqua Marine" fontColor="black" />
    <BonitaButton color="#9400D3" text="Dark Violet" />
  </header>
</template>

<script>
import BonitaButton from './Button.vue'

export default {
  name: 'Header',
  components: {
    BonitaButton,
  },
  props: {
    title: {
      type: String,
      default: 'Hueueue',
    },
  },
}
</script>
