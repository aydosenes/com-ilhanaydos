<template>
  <div class="about-card">
    <div class="card-title">
      <img src="settings.svg" alt="avatar" class="avatar" />
      <div class="title-text-content">
        <p>Hakkımızda</p>
        <h2>Projelerimiz</h2>
      </div>
    </div>
    <div class="card-content">
      <p>
        20 yıllık geçmişin bize verdiği güven ve tecrübeyle her türlü kazı,
        kırım, yıkım, çevre düzenleme ve peyzaj işlerini uygulama esaslarına
        göre titizlikle yapmaktayız. Müşteri odaklı çalışma prensibini
        benimseyerek, müşterilerimiz için en uygunu ve doğrusunu yapmaya
        çalışıyoruz. Bu amaçlar geçmiş tecrübelerimize de dayanarak
        müşterilerimize en uygun malzeme, işçilik ve fiyat teklifinde
        bulunuyoruz.
      </p>
      <table style="width:100%">
        <tr>
          <th>Hizmetler</th>
          <th>Çözümler</th>
        </tr>
        <tr>
          <td>Kazı</td>
          <td>Bünyemizdeki ekskavatör ve diğer iş makinlerini kullarak temiz bir iş çıkartmaktayız.</td>
        </tr>
        <tr>
          <td>Kırım - Yıkım</td>
          <td>Kırıcılarımızı büyük bir titizlik ile kullanıp aynı şekilde yıkım gerçekleştirmekteyiz.</td>
        </tr>
        <tr>
          <td>Tadilat</td>
          <td>Şantiye, hafriyat vs. kurulumu ve kurulum sonrasında gerekli tadilatları yapmaktayız.</td>
        </tr>
        <tr>
          <td>Çevre Düzenleme</td>
          <td>Bahçe, site içi düzenleme ve arazi düzenlemelerinde bulunmaktayız.</td>
        </tr>
        <tr>
          <td>Peyzaj ve Sulama</td>
          <td>Belediyelere refüjler arası veya yol kenarları peyzaj işleri ve otomatik sulama sistemleri sağlamaktayız.</td>
        </tr>
      </table>
    </div>
    <div class="footer">
      <a href="https://github.com/aydosenes" target="_blank" class="link"> aydosenes </a>
      <a class="link">© 2020</a>
    </div>
  </div>
</template>

<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-181920173-1">
</script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-181920173-1');
</script>
<!-- Global site tag (gtag.js) - Google Analytics -->


<style lang="sass" scoped>
.footer
  font-size: small
  text-align: center
.link
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
