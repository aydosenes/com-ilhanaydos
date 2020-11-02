<template>
  <div class="about-card">
    <div class="card-title">
      <img
        src="https://i.pinimg.com/originals/d3/69/d9/d369d9056795f553e244da66e8297cca.png"
        alt="avatar"
        class="avatar"
      />
      <div class="title-text-content">
        <p>Operatör</p>
        <h2>İlhan Aydos</h2>
      </div>
    </div>
    <div class="card-content">
      <p>
        ilhanaydos@outlook.com<br /><br />
        Peçenek Mah., Pursaklar / ANKARA
      </p>
      <p>
        <img src="whatsapp-logo.svg" width="15" height="15" alt="logo" />
        <a class="phone" href="https://wa.link/9nltwj" target="_blank"
          >+90532 320 48 00</a
        >
        <br />
        <br />
        <img src="whatsapp-logo.svg" width="15" height="15" alt="logo" />
        <a class="phone" href="https://wa.link/488h2p" target="_blank"
          >+90555 035 14 53</a
        >
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="sass" scoped>
.phone
    color: white
.about-card
  min-height: calc(100vh - 150px)
  background: #333
  padding: 3em
  border-radius: 10px
  color: white
  .card-title
    display: flex
    align-items: center
    background: #222
    border-radius: 10px
    .avatar
      height: 50px
      border: 1px solid rgba(255, 255, 255, 0.4)
      border-radius: 50%
      margin: 0 30px
  .title-text-content p
    margin-bottom: 0
    color: rgb(210, 210, 210)
  .title-text-content h2
    margin-top: 0
.card-content p
  line-height: 1.5
  margin: 30px auto
table
  border-spacing: 0px
  margin: 50px auto
  tr th, tr td
    border: 1px solid white
    border-top: none
    padding: 10px
    text-align: center
    &:first-of-type
      border-left: none
    &:nth-of-type(2)
      border-right: none
@media screen and (max-width: 530px)
  .about-card
    padding: 1em
  .card-title h2
    font-size: 1.3em
</style>
