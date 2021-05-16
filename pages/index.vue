
<template>
  <div class="center examplex">
    <vs-navbar
      target-scroll="#hide-scroll-content"
      hide-scroll
      center-collapsed
      v-model="active"
    >
      <template #left>
        <p class="title">blog.qqey.net</p>
      </template>

      <vs-navbar-item :active="active == 'top'" id="top">Top</vs-navbar-item>
      <vs-navbar-item :active="active == 'docs'" id="docs">
        docs
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'about'" id="about">
        About
      </vs-navbar-item>

      <template #right>
        <vs-button icon color="twitter">
          <i class="bx bxl-twitter"></i>
        </vs-button>
        <vs-button icon color="tumblr">
          <i class="bx bxl-github"></i>
        </vs-button>
      </template>
    </vs-navbar>
    <div id="hide-scroll-content" class="square"></div>
  </div>
</template>
<script>
export default {
  data: () => ({
    active: "top",
  }),
};
</script>



<style>
.title {
  font-weight: bold;
}
</style>
