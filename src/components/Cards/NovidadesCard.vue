<template>
  <div class="container-wrapper">
    <div class="container">
      <img :src="Novidade.img" alt="Avatar" class="image" />
      <div class="middle">
        <div class="text">Compre Agora</div>
      </div>
    </div>
    <p class="text-description">Lorem ispum dolor summit</p>
    <p class="text-price">99x de R$ 99,99</p>
  </div>
</template>
<script>
export default {
  props: ["Novidade"],
};
</script>
<style scoped>
.container-wrapper {
  padding: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 300px;
}
.container {
  position: relative;
  width: 300px;
}

.image {
  opacity: 1;
  display: block;
  width: 300px;
  height: 200px;
  object-fit: cover;
  transition: 0.5s ease;
  backface-visibility: hidden;
}

.middle {
  transition: 0.5s ease;
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  text-align: center;
}

.container:hover .image {
  opacity: 0.3;
}

.container:hover .middle {
  opacity: 1;
}

.text {
  cursor: pointer;
  background-color: orange;
  color: white;
  font-size: 13px;
  width: 100px;
  padding: 25px;
}
.text-description,
.text-price {
  font-family: inter !important;
  color: gray !important;
  font-weight: 400 !important;
}
.text-price {
  font-weight: 600 !important;
  margin-top: -12px;
}
</style>
