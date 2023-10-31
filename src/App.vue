<template>

 
<homepage/>
<first_page/>
<blook/>
<hr>

<product4/>
</template>



<script>
import HelloWorld from './components/HelloWorld.vue'
import homepage from './components/homepage.vue'
import first_page from './components/first_page.vue'
import Blook from './components/blook.vue'
import productDetails from './components/productDetails.vue'

import product4 from './components/stand/prodject4.vue'



export default {
  name: 'App',
  components: {

    homepage,
    first_page,
    Blook,
    productDetails,
    product4
  }

}
</script>

<style lang="scss"></style>
