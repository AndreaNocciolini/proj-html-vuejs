<template>
  <footer>
      <UpperFooter :upperFooterLinks="upperFooterLinks" :upperFooterSocial="upperFooterSocial" />
      <BottomFooter />  
  </footer>
</template>

<script>
import UpperFooter from './footer_components/UpperFooter.vue'
import BottomFooter from './footer_components/BottomFooter.vue'
export default {
    name: "Footer",
    components: {
        UpperFooter,
        BottomFooter
    },
    data() {
        return {
            upperFooterLinks: {
                0: {
                    link: 'HOME'
                },
                1: {
                    link: 'ABOUT'
                },
                2: {
                    link: 'PROJECTS'
                },
                3: {
                    link: 'SERVICES'
                },
                4: {
                    link: 'BLOG'
                },
                5: {
                    link: 'CONTACTS'
                },
            },
            upperFooterSocial: {
                0: {
                    icon: 'fab fa-instagram',
                },
                1: {
                    icon: 'fab fa-linkedin-in',
                },
                2: {
                    icon: 'fab fa-facebook-f',
                },
                3: {
                    icon: 'fab fa-twitter',
                },
            }
        }
    }
}
</script>

<style lang="scss" scoped>
    footer{
        width: 100%;
        background-color: var(--bg-dark-3);
    }
</style>