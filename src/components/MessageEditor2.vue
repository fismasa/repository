<template>

    <textarea ref="textAre" @change="onChange($event)">

    </textarea>
    <button @click="onSendClick()">
        Enviar
    </button>


</template>

<script lang="ts">
export default {
    data() {
        return {
            message: ''
        }
    },
    methods: {
        onChange(event: any) {
          
            
            this.message = event.target.value

        },

        onSendClick() {
            this.$emit('send', this.message);
            this.message = '';
           
        }
    }
}
</script>