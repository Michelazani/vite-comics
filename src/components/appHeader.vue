<script >
export default{
    name: 'appHeader',
    data() {
        return {
            navLinks : [
                {
                    content: 'Characters',
                    url: '#',
                    active: false,
                },

                {
                    content: 'Comics',
                    url: '#',
                    active: true,
                },

                {
                    content: 'Movies',
                    url: '#',
                    active: false,
                },

                {
                    content: 'Tv',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Games',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Collectibles',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Videos',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Fans',
                    url: '#',
                    active: false,
                },
                {
                    content: 'News',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Shop',
                    url: '#',
                    active: false,
                }
            ],
        }
    }
}
</script>

<template>
    <header>
        <section class="logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </section>
        <section class="nav">
            <ul>
                <li v-for="link in navLinks" :class="(link.active) ? 'active' : ''">
                    <a :href="link.url">{{link.content}}</a>
                 </li>
            </ul>
        </section>
    </header>
</template>

<style lang="scss" scoped>
  @use '../style/general.scss' as *; 
  @use '../style/partials/mixins' as *;

  header{
    @include flex (row, space-between , center);
    margin: 2rem 0;

    section.logo img{
        width: 70px;
        margin-left: 15rem;        
    }
    section.nav>ul{
        @include flex (row, center, center );
        margin-right: 15rem;
    }
    section.nav>ul li{
        padding: 1rem;
        text-transform: uppercase;
        font-size: 0.8rem;
    }
  }


</style>
