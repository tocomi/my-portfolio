<template lang="pug">
  div.artifact
    div.header
      span.title {{ artifact.title }}
      a.link(:href="artifact.link" target="_blank")
    div.content
      p.description {{ artifact.description }}
      h4 skill
      p.skill {{ artifact.skill }}
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
  margin: 10px auto;
  max-width: 600px;
  border-radius: 5px;
  .header {
    position: relative;
    padding: 10px;
    border-radius: 10px 10px 0 0;
    background-color: #EA8A2A;
    .title {
      font-size: 20px;
      font-weight: bold;
      text-decoration: none;
      color: #FFFFFF;
    }
    .link {
      position: absolute;
      top: 0;
      left: 0;
      height:100%;
      width: 100%;
    }
  }
  .content {
    padding: 16px;
    border-radius: 0 0 10px 10px;
    background-color: #EAEAEA;
    .description {
      margin: 0;
    }
    .skill {
      margin: -20px 0 0 0;
    }
    .icon {
      margin: 20px 0 0 0;
      height: 50px;
      width: 50px;
    }
  }
}
</style>
