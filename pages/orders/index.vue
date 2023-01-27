<template>
  <div>
    <h1>Orders Index Page works</h1>
    {{ orders }}
  </div>
</template>

<script>
export default {
  name: 'OrdersPage',
  components: {},
  async asyncData({$axios}){
    const orders = await $axios.$get('orders');
    return {
      orders,
    }
  },
  data(){
    return{}
  }
}
</script>
