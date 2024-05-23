<template>
<div>
    <input v-model="message" />
<button @click="$emit('send', message)">Emitir evento

</button>
</div>
</template>

<script lang="ts">
export default {

    data() {
        return {
            message: null
        }
    },
    methods: {
        send(){
            this.$emit('send', this.message)
        }
    }
}
</script>