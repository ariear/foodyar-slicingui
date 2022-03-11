<template>
  <Navbar />
  <Main />
  <MenuFood />
  <Testimoni />
  <Download />
  <Footer />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Main from "./components/Main.vue";
import MenuFood from "./components/MenuFood.vue";
import Testimoni from "./components/Testimoni.vue";
import Download from "./components/Download.vue";
import Footer from "./components/Footer.vue";
export default {
    components: { Navbar, Main, MenuFood, Testimoni, Download, Footer }
}
</script>