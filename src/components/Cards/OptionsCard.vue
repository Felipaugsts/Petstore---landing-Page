<template>
  <div class="containers">
    <img class="imgoption" :src="img" />
    <div class="txtdog">{{ text }}</div>
  </div>
</template>
<script>
export default {
  props: ["text", "img"],
};
</script>
<style scoped>
.containers {
  padding-right: 10px;
  position: relative;
  text-align: center;
  color: white;

  width: 370px;
}
.imgoption {
  width: 380px;
  object-fit: cover;
  height: 300px;
}
.txtdog {
  background: orange;
  width: auto;
  color: white;
  padding: 10px;

  position: absolute;
  top: 0px;
  right: 0px;
}
</style>
