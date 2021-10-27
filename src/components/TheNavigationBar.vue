<template>
  <div>
    <div id="nav">
      <div class="mobile">
        <i v-if="mobile" @click="OpenMobile" class="bi bi-list icon"></i>
        <i v-if="!mobile" @click="OpenMobile" class="bi bi-x icon"></i>
      </div>

      <input type="text" label="test" class="field" />
      <img
        class="logo"
        src="https://i.pinimg.com/originals/a9/8f/3e/a98f3e1cc96cfba875cca1b1dfd446ca.png"
      />
      <div class="icon-wrapper">
        <i class="bi bi-person icon person"></i>
        <i class="bi bi-cart icon cart"></i>
      </div>
    </div>
    <div
      :class="mobile ? 'hide-wrapper' : 'text-wrapper'"
      style="background: rgb(155, 51, 155)"
    >
      <div class="subNav">
        <div v-for="(opt, index) in navibar" :key="index">
          <p>{{ opt.name }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      mobile: false,
      navibar: [
        { name: "Categoria Lorem" },
        { name: "Categoria " },
        { name: "Categoria Lorem" },
        { name: "Categoria " },
        { name: "Categoria Lorem" },
      ],
    };
  },
  methods: {
    OpenMobile() {
      this.mobile = !this.mobile;
    },
    onResize() {
      if (window.innerWidth <= 520) {
        this.mobile = true;
      } else {
        this.mobile = false;
      }
    },
  },
  mounted() {
    this.$nextTick(() => {
      window.addEventListener("resize", this.onResize);
    });
  },

  beforeDestroy() {
    window.removeEventListener("resize", this.onResize);
  },
};
</script>
<style scoped></style>
