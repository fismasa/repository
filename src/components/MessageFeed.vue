<template>
    <div>
        <p v-for="(m, i) in messages">
            {{ m }}

        </p>
    </div>

</template>
<script lang="ts">
export default {
    props: {
        messages: {
            type: Array,
            required: true
        }

        
    }
}
</script>