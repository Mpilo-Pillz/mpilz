<template>
  <nav class="nav">
    <ul>
      <router-link to="/learning">
        <li>learning</li>
      </router-link>
      <router-link to="/projects">
        <li>projects</li>
      </router-link>

      <router-link to="/career">
        <li>career summary</li>
      </router-link>

      <router-link to="/" active-class="mobile-nav__item--cta">
        <li>home</li>
      </router-link>
    </ul>
  </nav>
</template>
<script>
export default {
  name: "appNavigator",
};
</script>
<style lang="scss" scoped>
.mobile-nav__item--cta {
  color: red;
  font-weight: bold;
  font-size: 2rem;
}
</style>
