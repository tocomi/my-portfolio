<template lang="pug">
  div#artifacts
    h1 Artifacts
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
        link: 'https://umaaji-calculator.firebaseapp.com/',
        github: 'https://github.com/tocomi/umaaji-calculator',
      },
    ]

  }
</script>

<style lang="scss" scoped>
</style>
