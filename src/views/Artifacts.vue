<template lang="pug">
  div#artifacts
    h2 Artifacts
    Artifact(v-for="artifact in this.artifacts" :artifact="artifact")
</template>

<script lang="ts">
  import { Component, Vue } from "vue-property-decorator"
  import Artifact from '../components/Artifact.vue'
  
  @Component({
    components: {
      Artifact,
    },
  })
  export default class Index extends Vue {

    artifacts: Array<any> = [
      {
        title: 'Umaaji-Calculator',
        description: '競馬の予想アプリです。過去の成績から各馬のスコア(ウマ味)を算出します。',
        skill: 'Vue.js, firebase, (Python)',
        link: 'https://umaaji-calculator.firebaseapp.com/',
        github: 'https://github.com/tocomi/umaaji-calculator',
      },
      {
        title: 'koedame',
        description: 'Twitterのオマージュ。つぶやきに偉人たちが反応してくれます。',
        skill: 'Vue.js, firebase',
        link: 'https://tocomi-koedame.firebaseapp.com/',
        github: 'https://github.com/tocomi/koedame',
      },
      {
        title: 'Smash-Memo',
        description: 'スマブラ用に特化したメモアプリ。(現状Androidのみ。Expoアプリのインストールが必要。)',
        skill: 'React Native',
        link: 'https://expo.io/@tocomi/smash-memo',
        github: 'https://github.com/tocomi/smash-memo',
      },
      {
        title: 'Portfolio',
        description: '今まさに開いているこれです',
        skill: 'Vue.js, firebase',
        link: 'https://tocomi-portfolio.web.app/',
        github: '',
      },
      {
        title: 'tekkaba',
        description: '競馬の予想共有アプリです。各ユーザーが登録した予想を共有します。',
        skill: 'Ruby on Rails, Vue.js, heroku',
        link: 'https://tekkaba.herokuapp.com/',
        github: 'https://github.com/tocomi/tekkaba',
      },
    ]

  }
</script>

<style lang="scss" scoped>
#artifacts {
  margin: 0 16px;
}
</style>
