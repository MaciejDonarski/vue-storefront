<template>
  <div>
    Core product row
  </div>  
</template>

<script>
import AddToCart from 'src/components/core/AddToCart.vue'
import { thumbnail } from 'src/lib/filters'

export default {
  name: 'product',
  props: ['product'],
  computed: {
    thumbnail () {
      return thumbnail(this.product.image, 150, 150)
    }
  },
  components: {
    AddToCart
  }
}
</script>

