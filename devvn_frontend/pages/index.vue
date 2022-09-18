<template>
  <div class="main-taiwinds">
      <div class="container">
          <Product v-for="product in products.data" :key="product.id" :product="product"/>
          <News />
      </div>
    </div>
</template>
<script setup>
  const { data: products } = await useFetch('http://localhost:1337/api/products?populate=*')
</script>

<script>

  import Product from '@/components/Products/Home/Product-Lists.vue'
  export default {
    components: {
        Product
    }
  }
</script>