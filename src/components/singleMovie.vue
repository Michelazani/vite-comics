<script >
export default {
    name: 'singleMovie',
    props: [
    'image',
    'series'
    ]
}
</script>

<template>
    <article>
        <img :src="image" alt="">
        <p>{{ series }}</p>
    </article>
</template>

<style lang="scss" scoped>
  @use '../style/general.scss' as *; 
  @use '../style/partials/variables' as *;
  @use '../style/partials/mixins' as *;

  article{
    width: calc((100% / 6) - 0.5rem);
    margin: 3rem 0.25rem 0 0.25rem;
    img{
        width: 150px;
        height: 170px;
    }
    p{
        text-transform: uppercase;
        color: $white;
        padding: 1rem 0;
    }
  }

</style>
