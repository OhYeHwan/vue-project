<template>
  <p>{{ name }}</p>
</template>

<script>
export default {
  props: ["name"],
};
</script>

<style scoped>
p {
  cursor: default;
  margin: 10px 0px 10px 0px;
  color: #fff;
  font-size: 60px;
}
</style>
