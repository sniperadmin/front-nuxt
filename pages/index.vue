<template>
  <div>
    <b-jumbotron class="p-4">
      <template v-slot:header>
        <b-row align-h="center">
          <Logo />
          nuxt-mall
        </b-row>
      </template>
      <template v-slot:lead>
        <div class="container">
          <p class="my-4">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit.
            Quod harum placeat consequatur animi eaque amet quae numquam vitae voluptates,
            temporibus dolorum necessitatibus perspiciatis blanditiis illo inventore porro corrupti libero molestiae?
          </p>
        </div>
      </template>
      <div class="container">
        <hr class="my-4">
        <p class="my-4">
          It uses utility classes for typography and spacing to space content out within the larger
          container.
        </p>
      </div>
      <div class="container">
        <b-row align-h="center">
          <h2 class="mb-2">
            Click below for the latest restaurants
          </h2>
        </b-row>
        <b-row align-h="center" class="my-4">
          <nuxt-link :to="{ name: 'restaurants-home' }">
            <Card style="width:320px">
              <div style="text-align:center">
                <Icon type="md-pizza" size="40" />
                <p>Go to Restaurants</p>
              </div>
            </Card>
          </nuxt-link>
        </b-row>
      </div>
    </b-jumbotron>
    <div class="container">
      <footer class="text-center my-5 mt-2">
        Project created by
        <a href="https://forums.coretabs.net/u/sniperadmin">
          Nasr Galal
        </a>
      </footer>
    </div>
  </div>
</template>
<script>
import Logo from '@/components/Logo.vue'
export default {
  components: {
    Logo
  }
}
</script>
