<template>
  <section class="nav">
    <div class="nav-logo">
      <img src="excavator-logo.png" width="100" height="100" alt="logo" />
      <br />
      <a><b>İlhan AYDOS</b></a>
      <br />
      <a>Kiralık İş Makineleri</a>
    </div>
    <div class="nav-menu">
      <ul class="nav-menu-list">
        <li class="nav-list-item" v-on:click="home">Ana Sayfa</li>
        <li class="nav-list-item" v-on:click="about">Hakkımızda</li>
        <li class="nav-list-item" v-on:click="contact">İletişim</li>
      </ul>
    </div>
    <div class="footer">
      <a href="https://github.com/aydosenes" target="_blank" class="link"> aydosenes </a>
      <a>© 2020</a><br />
    </div>
  </section>
</template>

<script>
import router from "@/router/index.js";
export default {
  methods: {
    home() {
      router.push({ path: "/" });
    },
    about() {
      router.push({ path: "about" });
    },
    contact() {
      router.push({ path: "contact" });
    }
  }
};
</script>

<style lang="sass" scoped>
.gitlogo
  display: block
  margin-left: auto
  margin-right: auto
  width: 30%
.nav
    position: fixed
    display: flex
    flex-direction: column
    align-items: center
    background: #D0D3D4
    top: 0
    left: 0
    bottom: 0
    width: 20vw
.nav-logo
    margin: 100px auto
    text-align: center
.nav-menu
    color: white
.nav-menu-list
    list-style: none
    padding: 0
.nav-list-item
    background: #222
    padding: 10px 20px
    text-align: center
    margin: 10px auto
    cursor: pointer
    &:hover
        width: 90%
.footer
    font-size: small
    text-align: center
.link
  color: black
</style>
