<template>
  <div class="mt-3">
    <Restaurants />
  </div>
</template>

<script>
import Restaurants from '@/components/Restaurants.vue'

export default {
  components: {
    Restaurants
  },
  computed: {
    filtered () {
      return this.restaurants.filter((restaurant) => {
        return restaurant.name.toLowerCase().includes(this.query.toLowerCase())
      })
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
