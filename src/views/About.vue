<template>
  <div>
    <b-container style="min-height: 100vh; padding-bottom: 50px">
      <b-row align-h="center" class="text-center">
        <b-col sm="12">
          <h1>
            About me
          </h1>
        </b-col>

        <b-col sm="12" md="4" style="padding: 30px 0">
          <img src="@/assets/me.png" alt="me" width="100%">
        </b-col>

        <b-col sm="12">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. A voluptates libero magni, quisquam in quibusdam, esse quo recusandae dolore aperiam nulla laudantium labore unde amet id consequuntur vitae veniam corporis inventore, consequatur modi! Id iure consequuntur tempore veritatis officiis hic vel excepturi nesciunt culpa doloribus, exercitationem totam voluptatum eius odit!
          </p>

          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus, blanditiis ex. Id numquam dolorum magnam sequi esse aliquam? Nostrum amet iure asperiores earum laborum mollitia facere tempora dignissimos, autem, veritatis libero corrupti ex quisquam at iusto, necessitatibus quasi! Veritatis, autem.
          </p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis cupiditate vero saepe corporis cum fugit unde facilis ducimus modi ea ullam dolore, autem ab. Laborum quod quisquam voluptate ullam alias similique ipsum molestiae iusto sed ab deleniti, quasi quo provident perferendis tempore eum. Cumque, excepturi nulla. Aliquid repellendus reiciendis deserunt!
          </p>
        </b-col>
      </b-row>

      <navbar />
    </b-container>
  </div>
</template>

<script>

import Navbar from '../components/Navbar.vue';

export default {
  components: {
    Navbar
  }
}
</script>

<style scoped>
  * {
    color: rgba(255, 255, 255, .75)
  }

</style>