<template>
    <Cards>
        <template #imagen>
            <img src="https://picsum.photos/id/1015/300" />

        </template>
        <template #titulo>
            <h2>Foto de vacaciones</h2>
        </template>
        <template #descripcion>
            <p>Aqui se puede describir los contenidos de la foto</p>

            <p>
                Por ejemplo tome esta foto en un paisaje
            </p>
        </template>

    </Cards>

</template>
<script lang="ts">
import Cards from './components/Cards.vue';

export default {
    components: {
        Cards
    }
}
</script>