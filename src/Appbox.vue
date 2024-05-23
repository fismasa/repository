<template>
<Box>
  <h3>Esta etiqueta h3 esta renderizada en el slot {{ count }}</h3>
  <button @click="count++">Incrementar </button>
</Box>
</template>

<script lang="ts">
import Box from './components/Box.vue';

export default{
  components: {
    Box
},

data() {
return {
  count: 0
}
}

}
</script>
