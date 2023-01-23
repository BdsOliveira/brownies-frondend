<template>
  <div>
    <div>
      <h1>
        Edit Product works!
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
  name: 'ProductEdit',
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
