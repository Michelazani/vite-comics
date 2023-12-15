<script >
export default{
    name: 'appBg',
    data() {
        return {

        }
    }
}
</script>

<template>
    <img src="../assets/img/jumbotron.jpg" alt="">
</template>

<style lang="scss" scoped>
  @use '../style/general.scss' as *; 
  @use '../style/partials/mixins' as *;

    img{
    width: 100%;
    height: 350px;
    object-fit: cover;
    object-position: top;
    }


</style>
