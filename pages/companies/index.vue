<template>
  <div>
    <h1>Companies Index Page works</h1>
    {{ companies }}
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: 'CompanyPage',
  components: {},
  async asyncData({$axios}){
    const companies = await $axios.$get('companies');
    return {
      companies,
    }
  },
  data(){
    return {
    }
  },
})
</script>
