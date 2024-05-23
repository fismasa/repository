<template>
    <MessageFeed :messages="messages" />
    <MessageEditor2 @send="onSend($event)" />

</template>

<script lang="ts">

import MessageFeed from './components/MessageFeed.vue';
import MessageEditor2 from './components/MessageEditor2.vue';

export default{

    components: {
        MessageFeed,
        MessageEditor2
    },

    data() {
        return{
            messages: [] as any
        }
    },

    methods: {
        onSend(event: any) {
            console.log(this.messages);
            this.messages = [...this.messages, event];
        }
    }



}
</script>