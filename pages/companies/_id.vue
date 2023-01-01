<template>
  <div>
    <div>
      <h1>
        Edit Company works!
        <h2>
          {{ id }}
        </h2>
      </h1>
    </div>
  </div>
</template>
<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'CompanyId',
  components: {},
  data() {
    const id = ref()
    return {
      id,
    }
  },
  mounted() {
    this.id = this.$route.params.id
  },
})
</script>
