<template>
  <div id="app">
    <desktop-nav id="desktop-nav" />
    <mobile-nav id="mobile-nav" />
    <div class="view-container">
      <router-view />
    </div>
  </div>
</template>

<script>
import DesktopNav from "@/components/DesktopNav.vue";
import MobileNav from "@/components/MobileNav.vue";
export default {
  components: {
    DesktopNav,
    MobileNav
  }
};
</script>

<style lang="sass" scoped>
.space
  background: #C0C0C0
.view-container
  width: 77vw
  padding: 1.5em
  margin-left: 22vw
  box-sizing: border-box
  min-height: 100vh
#mobile-nav
  display: none
@media screen and (max-width: 1096px)
  .view-container
    width: 100%
    margin-left: 0
  #desktop-nav
    display: none
  #mobile-nav
    display: flex
</style>
