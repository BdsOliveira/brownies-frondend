<template>
  <div>
    <h1>Companies Index Page works</h1>
    <div class="" v-for="company in companies" :key="company.id">
      <h1>{{ company.name }}</h1>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: 'CompanyPage',
  components: {},
  data(){
    const companies = fetch('http://localhost:8000/api/companies')
      .then(function(response) {
        return response.blob();
      })
    return {
      companies
    }
  },
})
</script>
