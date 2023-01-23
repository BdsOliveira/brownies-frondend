<template>
  <div class="h-screen bg-[#1F2937] text-white">
    <div class="container w-full">
        <div class="p-4 bg-[#111827] rounded">
          <NuxtLink class="flex" to="/">
            <div class="text-4xl">
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zM7.68 14.98H6V9h1.71c1.28 0 1.71 1.03 1.71 1.71v2.56c0 .68-.42 1.71-1.74 1.71zm4.7-3.52v1.07H11.2v1.39h1.93v1.07h-2.25c-.4.01-.74-.31-.75-.71V9.75c-.01-.4.31-.74.71-.75h2.28v1.07H11.2v1.39h1.18zm4.5 2.77c-.48 1.11-1.33.89-1.71 0L13.77 9h1.18l1.07 4.11L17.09 9h1.18l-1.39 5.23z"></path><path fill="currentColor" d="M7.77 10.12h-.63v3.77h.63c.14 0 .28-.05.42-.16c.14-.1.21-.26.21-.47v-2.52c0-.21-.07-.37-.21-.47a.72.72 0 0 0-.42-.15z"></path></svg>
            </div>
            <div class="px-2">

            </div>
          </NuxtLink>
        </div>
      </div>
    <div class="my-5">
      <div class="container w-full p-1 px-2">
        <div class="p-2 hover:bg-[#111827] rounded">
          <NuxtLink class="flex" to="/">
            <div class="text-2xl">
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="m12 5.69l5 4.5V18h-2v-6H9v6H7v-7.81l5-4.5M12 3L2 12h3v8h6v-6h2v6h6v-8h3L12 3z"></path></svg>
            </div>
            <div class="px-2">
              Dashboard
            </div>
          </NuxtLink>
        </div>
      </div>
      <div class="container w-full p-1 px-2">
        <div class="p-2 hover:bg-[#111827] rounded">
          <NuxtLink class="flex" to="/orders">
            <div class="text-2xl">
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="m21.41 11.41l-8.83-8.83c-.37-.37-.88-.58-1.41-.58H4c-1.1 0-2 .9-2 2v7.17c0 .53.21 1.04.59 1.41l8.83 8.83c.78.78 2.05.78 2.83 0l7.17-7.17c.78-.78.78-2.04-.01-2.83zM12.83 20L4 11.17V4h7.17L20 12.83L12.83 20z"></path><circle cx="6.5" cy="6.5" r="1.5" fill="currentColor"></circle></svg>
            </div>
            <div class="px-2">
              Vendas
            </div>
          </NuxtLink>
        </div>
      </div>
      <div class="container w-full p-1 px-2">
        <div class="p-2 hover:bg-[#111827] rounded">
          <NuxtLink class="flex" to="/companies">
            <div class="text-2xl">
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M1 11v10h6v-5h2v5h6V11L8 6l-7 5zm12 8h-2v-5H5v5H3v-6.97l5-3.57l5 3.57V19zm4-12h2v2h-2zm0 4h2v2h-2zm0 4h2v2h-2z"></path><path fill="currentColor" d="M10 3v1.97l2 1.43V5h9v14h-4v2h6V3z"></path></svg>
            </div>
            <div class="px-2">
              Empresas
            </div>
          </NuxtLink>
        </div>
      </div>
      <div class="container w-full p-1 px-2">
        <div class="p-2 hover:bg-[#111827] rounded">
          <NuxtLink class="flex" to="/sellers">
            <div class="text-2xl">
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M16.67 13.13C18.04 14.06 19 15.32 19 17v3h4v-3c0-2.18-3.57-3.47-6.33-3.87zM15 12c2.21 0 4-1.79 4-4s-1.79-4-4-4c-.47 0-.91.1-1.33.24a5.98 5.98 0 0 1 0 7.52c.42.14.86.24 1.33.24zm-6 0c2.21 0 4-1.79 4-4s-1.79-4-4-4s-4 1.79-4 4s1.79 4 4 4zm0-6c1.1 0 2 .9 2 2s-.9 2-2 2s-2-.9-2-2s.9-2 2-2zm0 7c-2.67 0-8 1.34-8 4v3h16v-3c0-2.66-5.33-4-8-4zm6 5H3v-.99C3.2 16.29 6.3 15 9 15s5.8 1.29 6 2v1z"></path></svg>
            </div>
            <div class="px-2">
              Vendedores
            </div>
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SidebarComponent',
  components: {
  },
  data() {
    return {
    }
  },
}
</script>
<style lang="sass" scoped>

</style>
