<template>
  <div>
    <div v-for="company in sellers" :key="company">
      <h1>{{ company[0].company.name }}</h1>
      <div v-for="seller in company" :key="seller.id">
        {{ seller.name }}
      </div>
    <br>
    <hr>
    <br>
    </div>
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
