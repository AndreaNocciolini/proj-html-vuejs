<template>
  <main>
      <Jumbo :icon="icon" />
      <Consultants :consultantsArray="consultantsArray"/>
  </main>
</template>

<script>
import Jumbo from './main_components/Jumbo.vue'
import Consultants from './main_components/Consultants.vue'

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
    }
}
</script>

<style lang="scss" scoped>
    
</style>