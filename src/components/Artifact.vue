<template lang="pug">
  div.artifact
    a.title(:href="artifact.link" target="_blank") {{ artifact.title }}
    p {{ artifact.description }}
    a(:href="artifact.github" target="_blank") github
</template>

<script lang="ts">
  import { Component, Prop, Vue } from "vue-property-decorator"
  
  @Component({
    components: {
    },
  })
  export default class Index extends Vue {

    @Prop() artifact!: any

  }
</script>

<style lang="scss" scoped>
.title {
  font-size: 24px;
  font-weight: bold;
  text-decoration: none;
}
</style>
