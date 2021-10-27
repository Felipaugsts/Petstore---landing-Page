<template>
  <div class="footer-container">
    <div class="wrp">
      <div class="item">
        <img
          class="logoimg"
          src="https://images.vexels.com/media/users/3/202044/isolated/lists/651fff530d4deddc530316c4172b7c9b-heart-dog-footprints-flat.png"
        />
        <p class="txtfoot">ENTREGA GRATUITA A PARTIR DE R$99</p>
      </div>
      <div class="item">
        <img
          class="logoimg"
          src="https://images.vexels.com/media/users/3/202044/isolated/lists/651fff530d4deddc530316c4172b7c9b-heart-dog-footprints-flat.png"
        />
        <p class="txtfoot">PARCELAMENTO SEM JUROS</p>
      </div>
      <div class="item">
        <img
          class="logoimg"
          src="https://images.vexels.com/media/users/3/202044/isolated/lists/651fff530d4deddc530316c4172b7c9b-heart-dog-footprints-flat.png"
        />
        <p class="txtfoot">GANHE DESCONTOS</p>
      </div>
    </div>
    <div class="item2">
      <h1 class="sign-txt">ASSINE NOSSA NEWSLETTER</h1>
      <h3 class="sub-txt">
        Cadastre-se para receber nossas novidades e descontos
      </h3>
      <div>
        <input type="email" class="fields" placeholder="Email" />
        <button class="button">Enviar</button>
      </div>
    </div>
  </div>
</template>
<style scoped>
.footer-container {
  width: 100%;
  height: 300px;
  background: rgb(148, 86, 230);
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}
.wrp {
  width: 80%;
  display: flex;
  height: 50px;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  justify-content: space-around;
}
.logoimg {
  height: 25px;
  margin-right: 5px;
}
.txtfoot {
  font-family: inter !important;
  font-weight: 400 !important;
  font-size: 12px !important;
  color: white;
}
.item {
  display: flex;
  justify-content: center;
  align-items: center;
}
.item2 {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.sign-txt,
.sub-txt {
  font-family: inter !important;
  color: white;
}
.sign-txt {
  font-size: 27px;
}
.sub-txt {
  font-weight: 400 !important;
  font-size: 16px;
  margin-top: -5px;
}
.button {
  height: 35px;
  padding-right: 10px;
  padding-left: 10px;
  background: orange;
  color: white;
  font-family: inter !important;
}
.fields {
  height: 30px;
  margin-top: 10px;
}
</style>
