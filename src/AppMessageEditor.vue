<template>
<div>
    <p>{{ parentMessage }}</p>


    <!--
    <MessageEditor @send="parentMessage = $event"/>
    -->

    <MessageEditor @send="updateParentMessage"/>

    <button @click="parentMessage=null">Reset</button>
</div>
</template>
<script lang="ts">
import MessageEditor from './components/MessageEditor.vue';

export default{

    components: {
        MessageEditor

    },

    data(){

        return {
        parentMessage: null
        }
    },

    methods: {
        updateParentMessage(newMessage: any) {
            this.parentMessage = newMessage;
        }
    }
}
</script>