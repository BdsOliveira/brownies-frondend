<template>
  <div class="flex flex-col p-16">
    <div class="flex flex-row flex-wrap gap-10 mb-8">
      <div class="bg-white rounded shadow">
        <RouterLink to="/sellers/">
        <div class="w-52 h-24 flex items-center justify-center">
          <div class="text-xl px-1">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="m12 5.69l5 4.5V18h-2v-6H9v6H7v-7.81l5-4.5M12 3L2 12h3v8h6v-6h2v6h6v-8h3L12 3z"></path></svg>
          </div>
          <div class="ml-2">
            Início
          </div>
        </div>
        </RouterLink>
      </div>
      <div class="bg-white rounded shadow">
        <RouterLink to="/sellers/new">
        <div class="w-52 h-24 flex items-center justify-center">
          <div class="text-xl px-1">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M19 12.998h-6v6h-2v-6H5v-2h6v-6h2v6h6z"></path></svg>
          </div>
          <div class="ml-2">
            Novo Vendedor
          </div>
        </div>
        </RouterLink>
      </div>
      <!-- <div class="bg-white rounded shadow">
        <RouterLink to="/sellers/ranking">
        <div class="w-52 h-24 flex items-center justify-center">
          <div class="text-xl px-1">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M19 12.998h-6v6h-2v-6H5v-2h6v-6h2v6h6z"></path></svg>
          </div>
          <div class="ml-2">
            Desempenho
          </div>
        </div>
        </RouterLink>
      </div> -->
      <div class="bg-white rounded shadow">
        <RouterLink to="/sellers/report">
        <div class="w-52 h-24 flex items-center justify-center">
          <div class="text-xl px-1">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M19 12.998h-6v6h-2v-6H5v-2h6v-6h2v6h6z"></path></svg>
          </div>
          <div class="ml-2">
            Gerar Relatório
          </div>
        </div>
        </RouterLink>
      </div>
    </div>
    <NuxtChild />
  </div>
</template>

<script>
export default {
  name: 'SellersLayout',
  components: {},
}
</script>
