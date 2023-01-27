<template>
  <div>
    <h1>Products Index Page works</h1>
    {{ products }}
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: 'ProductPage',
  components: {},
  async asyncData({$axios}){
    const products = await $axios.$get('products');
    return {
      products,
    }
  },
  data(){
    return {
    }
  },
})
</script>
