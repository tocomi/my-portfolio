<template lang="pug">
  div.artifact
    a.title(:href="artifact.link" target="_blank") {{ artifact.title }}
    p {{ artifact.description }}
    a(:href="artifact.github" target="_blank")
      img.icon(alt="github" src="../assets/github.png")
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
.artifact {
  .title {
    font-size: 24px;
    font-weight: bold;
    text-decoration: none;
  }
  .icon {
    height: 50px;
    width: 50px;
  }
}
</style>
