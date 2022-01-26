<template>
  <main>
      <Jumbo />
      <Consultants :consultantsArray ="consultantsArray"/>
      <AboutUs />
      <Projects :projectsArray ="projectsArray" />
      <Testimonials :commentsArray="commentsArray" />
      <Blog :articlesArray="articlesArray"/>
      <LetsTalk />
  </main>
</template>

<script>
import Jumbo from './main_components/Jumbo.vue'
import Consultants from './main_components/Consultants.vue'
import AboutUs from './main_components/AboutUs.vue'
import Projects from './main_components/Projects.vue'
import Testimonials from './main_components/Testimonials.vue'
import Blog from './main_components/Blog.vue'
import LetsTalk from './main_components/LetsTalk.vue'

export default {
    name: "Main",
    data(){
        return {
            consultantsArray: {
                0: {
                    icon: 'fas fa-chart-line',
                    title: 'STATISTICAL CONSULTING',
                    description:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                },
                1: {
                    icon: 'fas fa-bullhorn',
                    title: 'DIGITAL CONSULTING',
                    description:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                },
                2: {
                    icon: 'fas fa-wallet',
                    title: 'BANKING CONSULTING',
                    description:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                },
                3: {
                    icon: 'fas fa-bullseye',
                    title: 'ENTERPRISE CONSULTING',
                    description:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                }
            },
            projectsArray: {
                0: {
                    src: require('../assets/images/DRY-1-790x592.jpg'),
                    company: 'Purinky products',
                    product_category: 'uncategorized'
                },
                1: {
                    src: require('../assets/images/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg'),
                    company: 'Spelunky objects',
                    product_category: 'uncategorized'
                },
                2: {
                    src: require('../assets/images/z1el4c4p-790x592.jpg'),
                    company: 'Sarappa items',
                    product_category: 'uncategorized'
                }
            },
            commentsArray: {
                0: {
                    text: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a',
                    author: 'Vera Duncan',
                    company:'Amazon Inc.'
                },
                1: {
                    text: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a',
                    author: 'Stan Smith',
                    company:'Boolean Inc.'
                },
                2: {
                    text: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a',
                    author: 'Bill Gates',
                    company:'Microsoft Inc.'
                }
            },
            articlesArray: {
                0:{
                    src: require('../assets/images/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg'),
                    date:'July 4, 2019',
                    author:'paul',
                    title:'Canadian consulting firm acquired by UK giant',
                    content:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                },
                1:{
                    src: require('../assets/images/business-people-working-together-on-project-and-5FHSKBL-1390.jpg'),
                    date:'July 13, 2019',
                    author:'Beth',
                    title:'American consulting firm acquired by IT giant',
                    content:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                },
            }
        }
    },
    components: { 
        Jumbo,
        Consultants,
        AboutUs,
        Projects,
        Testimonials,
        Blog,
        LetsTalk
    }
}
</script>

<style lang="scss" scoped>
    
</style>