<template>
    <div>
        <Article>
            <template v-slot:titulo>
                <h3>mi titulo del articulo</h3>

            </template>
            <!--
            <template #extracto>
            -->
            <template v-slot:extracto>
                <p>Primer parrafo del contenido</p>
                <p>Segundo parrafo del contenido</p>
            </template>
        </Article>
    </div>

</template>

<script lang="ts">
import Article from './components/Article.vue';

export default {
    components: {
        Article
    }
}
</script>