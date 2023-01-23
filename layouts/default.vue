<template>
  <div class="container flex flex-row">
    <SidebarComponent />
    <div class="m-8">
      <HeaderComponent />
      <Nuxt />
      <FooterComponent />
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

