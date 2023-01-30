<template>
  <div>
    <div v-for="company in sellers" :key="company.id">
      <h1>{{ company[0].company.name }}</h1>
      <div class="flex flex-wrap">
        <div v-for="seller in company" :key="seller.id" class="m-2">
          <NuxtLink :to="`/sellers/${seller.id}`">
            {{ seller.name }}
          </NuxtLink>
        </div>
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
