<template lang="pug">
  div#sns
    h2 SNS
    a(href="https://twitter.com/tocomi0112" target="_blank")
      img#twitter.icon(alt="twitter" src="../assets/twitter.png")
    a(href="https://github.com/tocomi" target="_blank")
      img#github.icon(alt="github" src="../assets/github.png")
    a(href="https://qiita.com/tocomi" target="_blank")
      img#qiita.icon(alt="qiita" src="../assets/qiita.png")
    a(href="https://tocomi.hatenablog.com/" target="_blank")
      img#hatena.icon(alt="hatena" src="../assets/hatena.svg")
    a(href="https://www.facebook.com/kenta.tsunemi.5" target="_blank")
      img#facebook.icon(alt="facebook" src="../assets/facebook.png")
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  components: {
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
#sns {
  .icon {
    margin: 10px 15px 0 15px;
    height: 75px;
    width: 75px;
  }
}
</style>

