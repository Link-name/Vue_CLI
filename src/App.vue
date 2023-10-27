<template>

 
<homepage/>
<first_page/>
<blook/>
<hr>
<productDetails/>
</template>



<script>
import HelloWorld from './components/HelloWorld.vue'
import homepage from './components/homepage.vue'
import first_page from './components/first_page.vue'
import Blook from './components/blook.vue'
import productDetails from './components/productDetails.vue'

export default {
  name: 'App',
  components: {

    homepage,
    first_page,
    Blook,
    productDetails
  }

}
</script>

<style lang="scss"></style>
