<template>
  <div>
    <p v-if="age < 18">подросток</p>
    <p v-else-if="age >= 19 && age <= 25">молодой человек</p>
    <p v-else>мужчина</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      age: 25
    }
  }
}
</script>

<template>
  <table>
    <tr v-for="product in products" :key="products">
      <td>{{ product.name }}</td>
      <td>{{ product.price }}</td>
      <td>{{ product.quantity }}</td>
    </tr>
  </table>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          name: 'product1',
          price: 100,
          quantity: 5,
        },
        {
          name: 'product2',
          price: 200,
          quantity: 4,
        },
        {
          name: 'product3',
          price: 300,
          quantity: 3,
        },
      ]
    }
  }
}
</script>
