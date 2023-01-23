<template>
  <div class="flex flex-row bg-[#F3F4F6]">
    <SidebarComponent class="w-1/5"/>
    <div class="w-4/5">
      <!-- <HeaderComponent /> -->
      <Nuxt />
      <!-- <FooterComponent /> -->
    </div>
  </div>
</template>

<script>

export default {
  name: 'DefaultLayout',
  components: {
},
  data() {
    return {
    }
  },
}
</script>

<style scoped>
:root{
  --primary: #4ade80;
  --primary-alt: #22c55e;
  --grey: #64748b;
  --dark: #1e293b;
  --dark-alt: #334155;
  --light: #f1f5f9;
  --sidebar-width: 300px
}

</style>

