<script>
import AppNavbar from "./components/AppNavbar.vue";
import AppContent from "./components/AppContent.vue";
import AppBuy from "./components/AppBuy.vue"
import AppFooter from "./components/AppFooter.vue";
import AppFollow from "./components/AppFollow.vue";

export default{
  data(){
    return{};
  },
  components:{
    AppNavbar,
    AppContent,
    AppBuy,
    AppFooter,
    AppFollow
  },
};
</script>
<template>
  <AppNavbar></AppNavbar>
  <AppContent></AppContent>
  <AppBuy></AppBuy>
  <AppFooter></AppFooter>
  <AppFollow></AppFollow>
</template>
<style scoped></style>