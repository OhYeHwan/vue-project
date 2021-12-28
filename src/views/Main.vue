<template>
  <main>
    <Logo name="VUE.GG" />
    <Searchbar />
  </main>
</template>

<script>
import Logo from "@/components/Logo.vue";
import Searchbar from "@/components/Searchbar.vue";

export default {
  components: {
    Logo,
    Searchbar,
  },
};
</script>

<style scoped>
main {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: rgb(94, 130, 225);
}
</style>
