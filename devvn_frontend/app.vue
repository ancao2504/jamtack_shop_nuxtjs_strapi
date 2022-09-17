<template>
  <div>
    <Navbar />
    <div class="main-taiwinds">
      <div class="container">
          <Product />
          <News />
      </div>
    </div>
    
    <Footer />
  </div>
</template>

<script>
  import Product from '@/components/Products/Home/Product-Lists.vue'
  export default {
    components: {
        Product
    }
  }
</script>