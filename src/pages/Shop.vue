<template>
  <div class="wrapper-content wrapper-content--fixed">

    <section>
      <div class="container">
        <h1>Shop Page</h1>
        <ShopItem></ShopItem>
      </div>

    </section>

  </div>
</template>

<script>
import ShopItem from "../components/ShopItem";
export default {
  name: "Shop",
  components: {ShopItem},
  data () {
    return {
      shopList: null
    }
  },
  created() {
    this.shopList = this.$store.getters.getShopList
    console.log(this.shopList)
  }
}
</script>

<style scoped>

</style>