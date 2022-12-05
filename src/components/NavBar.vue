<template>
  <nav class="menu">
    <div class="menu-logo">
      <router-link to="/">
        Home
      </router-link>
    </div>
    <ul class="menu-links">
      <li class="menu-links-link">
        <router-link to="/form">Form</router-link>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss">
@import "@/assets/style/all.scss";

.menu {
  @include flex(row, nowrap, space-between, center);
  width: 100%;
  height: $nav;

  &-logo {
    position: relative;
    width: 75px;
    height: 75px;
    padding: $pad;

    img {
      width: 100%;
      height: 100%;
    }
  }

  &-links {
    @include flex(row, nowrap, space-between, center);

    &-link {
      margin: $pad;
    }
  }
}
</style>
