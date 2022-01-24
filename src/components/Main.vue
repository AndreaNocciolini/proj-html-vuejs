<template>
  <main>
      <Jumbo :icon="icon" />
      <Consultants :consultantsArray="consultantsArray"/>
      <AboutUs />
      <Projects /><!-- -----------RIPARTI DAL COMPONENT 'PROJECTS.VUE' IN 'MAIN_COMPONENTS' ****************** -->
  </main>
</template>

<script>
import Jumbo from './main_components/Jumbo.vue'
import Consultants from './main_components/Consultants.vue'
import AboutUs from './main_components/AboutUs.vue'
import Projects from './main_components/Projects.vue'

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
            }
        }
    },
    components: { 
        Jumbo,
        Consultants,
        AboutUs,
        Projects,
    }
}
</script>

<style lang="scss" scoped>
    
</style>