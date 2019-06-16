<template lang="pug">
  div#artifacts
    h1 Artifacts
    div.artifact(v-for="artifact in this.artifacts")
      a.title(:href="artifact.link" target="_blank") {{ artifact.title }}
      p {{ artifact.description }}
      a(:href="artifact.github" target="_blank") github
</template>

<script lang="ts">
  import { Component, Vue } from "vue-property-decorator"
  
  @Component({
    components: {
    },
  })
  export default class Index extends Vue {

    artifacts: Array<any> = [
      {
        title: 'Umaaji-Calculator',
        description: '競馬の予想アプリです。過去の成績から各馬のスコア(ウマ味)を算出します。',
        link: 'https://umaaji-calculator.firebaseapp.com/',
        github: 'https://github.com/tocomi/umaaji-calculator',
      },
    ]

  }
</script>

<style lang="scss" scoped>
.title {
  font-size: 24px;
  font-weight: bold;
  text-decoration: none;
}
</style>
