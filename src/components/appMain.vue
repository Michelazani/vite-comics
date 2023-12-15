<script >
export default{
}
</script>

<template>
    <main>
        <section>
            <h2> <i class="fa-solid fa-arrow-right" style="color: #ffffff;"></i> Content goes here <i class="fa-solid fa-arrow-left" style="color: #ffffff;"></i></h2>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins' as *;

main{
    h2{
        padding: 3rem 0 3rem 15rem;
        margin-bottom: 0;
    }
    i{
        margin: 0 1rem;
    }
}

</style>