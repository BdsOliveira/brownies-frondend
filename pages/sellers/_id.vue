<template>
  <div>
    <div>
      <table class="table">
        <thead>
          <tr>
            <th colspan="2">
              {{ seller.orders[0].seller.name }}
            </th>
            <th>
              {{ seller.orders[0].seller.company.name }} -
            </th>
            <th>
              {{ new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(seller.billing.amount) }}
            </th>
          </tr>
          <tr>
            <th>
              Produto Vendido
            </th>
            <th>
              Quantidade vendida
            </th>
            <th>
              Data
            </th>
            <th>
              Total vendido
            </th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="order in seller.orders" :key="order.id" class="">
            <td>
              {{ order.product.name }}
            </td>
            <td>
              {{ order.quantity }}
            </td>
            <td>
              {{ order.date }}
            </td>
            <td>
              {{ new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(order.product.price * order.quantity) }}
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'Seller',
  components: {},
  async asyncData({ $axios, route }) {
    const { id } = route.params
    const seller = await $axios.$get('sellers/' + id + "/orders")
    return {
      seller
    }
  },
  data() {
    return {
    }
  },
})
</script>
