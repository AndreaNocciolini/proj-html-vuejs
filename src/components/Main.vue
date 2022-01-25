<template>
  <main>
      <Jumbo :icon="icon" />
      <Consultants :consultantsArray ="consultantsArray"/>
      <AboutUs />
      <Projects :projectsImgArray ="projectsImgArray" />
      <Testimonials :commentsArray="commentsArray" />
  </main>
</template>

<script>
import Jumbo from './main_components/Jumbo.vue'
import Consultants from './main_components/Consultants.vue'
import AboutUs from './main_components/AboutUs.vue'
import Projects from './main_components/Projects.vue'
import Testimonials from './main_components/Testimonials.vue'

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
            projectsImgArray: {
                0: {
                    src: '../../assets/images/DRY-1-790x592.jpg'
                },
                1: {
                    src: '../../assets/images/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg'
                },
                2: {
                    src: '../../assets/images/z1el4c4p-790x592.jpg'
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
            }
        }
    },
    components: { 
        Jumbo,
        Consultants,
        AboutUs,
        Projects,
        Testimonials,
    }
}
</script>

<style lang="scss" scoped>
    
</style>