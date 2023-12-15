<script >

import listMovies from './listMovies.vue';
export default{
    name: 'appMain',
    components:{
        listMovies
    }
}
</script>

<template>
    <main>
        <section>
            <button class=" upper-button">
                current series
            </button>
            <listMovies/>
            <button class="bottom-button">Load more</button>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins' as *;

main{
    section{
        @include flex(column, center, center);
        position: relative;
        button{
        margin-bottom: 1rem;
        padding: 0.2rem 1.5rem;
        color: $white;
        background-color: $blue;
        border: none;
        &.upper-button{
            position: absolute;
            bottom: 635px;
            left: 225px;
        }
    }
    }
}

</style>