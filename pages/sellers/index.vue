<template>
  <div>
    <h1>Sellers Index Page works</h1>
    {{ sellers }}
  </div>
</template>

<script>
export default {
  name: 'SellerPage',
  components: {},
  async asyncData({$axios}) {
    const sellers = await $axios.$get('sellers');
    return {
      sellers
    };
  },
  data(){
    return {
    }
  }
}
</script>
