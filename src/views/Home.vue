<template>
  <div class="about-card">
    <vue-displacement-slideshow
      :images="images"
      displacement="require('../assets/displacement.png')"
      :intensity="0.2"
      :speedIn="1.0"
      :speedOut="1.0"
      ease="expo.out"
      ref="slideshow">
    </vue-displacement-slideshow>
  </div>
</template>

<script>
import VueDisplacementSlideshow from "vue-displacement-slideshow";

export default {
  components: {
    VueDisplacementSlideshow
  },
  computed: {
    images() {
      return [
        require('../assets/1.jpeg'),
        require('../assets/2.jpeg'),
        require('../assets/3.jpeg'),
        require('../assets/4.jpeg'),
        require('../assets/5.jpeg'),
        require('../assets/6.jpeg'),
        require('../assets/7.jpeg'),
        require('../assets/8.jpeg'),
        require('../assets/9.jpeg'),
        require('../assets/10.jpeg'),
        require('../assets/11.jpeg'),
        require('../assets/12.jpeg'),
        require('../assets/13.jpeg'),
        require('../assets/14.jpeg'),
        require('../assets/15.jpeg'),
        require('../assets/16.jpeg'),
        require('../assets/17.jpeg')
      ];
    },
  },
  methods: {
    init() {
        setInterval(() => {
        this.$refs.slideshow.next();
      }, 2000);
    },
  },
  mounted() {
    this.init();
  }
};
</script>
<style lang="sass" scoped>
.about-card
  min-height: calc(100vh - 150px)
  background: #333
  padding: 3em
  border-radius: 10px
  color: white
.card-content p
  line-height: 1.5
  margin: 30px auto
@media screen and (max-width: 530px)
  .about-card
    padding: 1em
  .card-title h2
    font-size: 1.3em
.vue-displacement-slideshow
  min-height: calc(100vh - 150px)
</style>
