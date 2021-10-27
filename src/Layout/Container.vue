<template>
  <div class="wrapper">
    <h1 class="info-text">{{ text }}</h1>
    <div :class="tipo === 'tog' ? 'tog' : 'container'">
      <slot class="child" />
    </div>
  </div>
</template>
<script>
export default {
  props: ["tipo", "text"],
};
</script>
<style scoped>
@import url("../assets/css/responsive.css");
.container {
  display: flex;
  justify-content: space-around !important;
  align-items: center;
  flex-wrap: wrap;
  width: 100%;

  width: 80%;
}
.tog {
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;

  width: 80%;
}
.wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.info-text {
  font-family: inter !important;
  color: gray;
}
.child {
  display: flex;
  flex-direction: column;
  flex-basis: 100%;
  flex: 1;
}
</style>
