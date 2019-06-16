<template lang="pug">
  div#artifacts
    h1 This is aritfacts page
    div.artifact(v-for="artifact in this.artifacts")
      p {{ artifact.title }}
      p {{ artifact.description }}
      p {{ artifact.link }}
      p {{ artifact.github }}
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
        description: 'あ\nい\nう',
        link: 'https://umaaji-calculator.firebaseapp.com/',
        github: 'https://github.com/tocomi/umaaji-calculator',
      },
    ]

  }
</script>