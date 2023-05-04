<script setup>
import { ref } from 'vue'
import MdEditor from 'md-editor-v3'
import 'md-editor-v3/lib/style.css'

const textContent = `
The mind is a labyrinth, ladies and gentlemen, a puzzle. And while the paths of the brain are plainly visible, its ways deceptively apparent, its destinations are unknown. Its secrets still secret, and, if we are honest, it is the lure of the labyrinth that draws us to our chosen field. To unlock those secrets. Others have been here before us and have left us signs, but we, as explorers of the mind, must devote our lives and energies to going further. To tread the unknown corridors in order to find ultimately, the final solution. We have to see. We have to know.

- Dr. Philip Channard, Hellbound: Hellraiser II
`

const text = ref(textContent)
</script>

<template>
  <MdEditor v-model="text" language="en-US" />
</template>
