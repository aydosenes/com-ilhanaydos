<template>
  <section class="nav">
    <div class="nav-logo">
      <img src="excavator-logo.png" width="100" height="100" alt="logo" />
      <br />
      <a><b>İlhan AYDOS</b></a>
      <br />
      <a>Kiralık İş Makineleri</a>
    </div>
    <div class="footer">
      <a href="https://github.com/aydosenes" target="_blank"> aydosenes </a>
      <a>© 2020</a>
    </div>
    <div class="nav-menu">
      <ul class="nav-menu-list">
        <li class="nav-list-item" v-on:click="home">Ana Sayfa</li>
        <li class="nav-list-item" v-on:click="about">Hakkımızda</li>
        <li class="nav-list-item" v-on:click="contact">İletişim</li>
      </ul>
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
.nav
    background: #D0D3D4
    display: flex
    flex-direction: column
    justify-content: space-around
    align-items: center
    text-align: center
.nav-logo
    margin: 20px auto
.nav-menu
    width: 100%
.nav-menu-list
    list-style: none
    padding: 0
    display: flex
    margin: 0
    color: white
li
    width: 50%
    text-align: center
    background: #555
    padding: 10px 0
    cursor: pointer
    transition: background 300ms ease-in-out
    &:hover
        background: #333
.footer
    font-size: small
    text-align: left
</style>
