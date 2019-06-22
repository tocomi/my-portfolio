<template lang="pug">
  div#about
    h2 About
    img#icon(alt="Vue logo" src="../assets/2896.jpg")
    div#introduction
      h3#name @tocomi
      div#text
        p 社会人になるのをきっかけにエンジニアになりました。
        p 個人でWebアプリケーションを開発するのが趣味です。
        h3 経歴
        p.bold 2010.04- 東北大学経済学部
        p.bold 2015.04- ワークスアプリケーションズ
        p - Webアプリケーションのバグ修正(Java,html,js,css)
        p - 社内ツールの開発・マネジメント(Java,AWS)
        h3 Skill
        p Java Ruby Rails Python JavaScript Vue.js ReactNative jQuery html pug css sass Delphi COBOL shell
        p EC2 cloudformation lambda firebase Jenkins Ansible Docker Oracle PostgreSQL
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
#about {
  #icon {
    border-radius: 50%;
    height: 100px;
    width: 100px;
  }
  #introduction {
    .bold {
      font-weight: bold;
    }
  }
}
</style>

