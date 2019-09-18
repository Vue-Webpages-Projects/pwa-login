<template>
  <div style="min-height: 100vh; padding-bottom: 50px">

      <b-container>
        <b-row align-h="center" style="padding: 30px 0">
            <!-- <b-col cols="6" class="padding">
                <div class="text-center">
                    <i class="fas fa-ghost icons"></i>
                </div>
            </b-col> -->

            <app v-for="app in apps"
                    v-bind:key="app.id"
                    v-bind:app="app"/>

        </b-row>
      </b-container>


    <navbar />
  </div>
</template>

<script>  
import Navbar from '@/components/Navbar.vue'
import App from '@/components/App.vue'

export default {
  name: 'home',
  components: {
    Navbar,
    App
  },
  data (){
      return {
          apps: [
              {
                  id: 99,
                  icon: 'fas fa-home icons',
                  name: 'Home'
              },
              {
                  id: 1,
                  icon: 'fas fa-ghost icons',
                  name: 'Ghost'
              },
              {
                  id: 2,
                  icon: 'fas fa-cogs icons',
                  name: 'Settings'
              },
              {
                  id: 3,
                  icon: 'fab fa-github-square icons',
                  name: 'Github'
              },
              {
                  id: 4,
                  icon: 'fab fa-facebook-square icons',
                  name: 'Facebook'
              },
              {
                  id: 5,
                  icon: 'fas fa-beer icons',
                  name: 'Beer'
              },
              {
                  id: 6,
                  icon: 'fas fa-bolt icons',
                  name: 'Bolt'
              }
          ]
      }
  }
}
</script>

<style scoped>


</style>