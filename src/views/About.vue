<template lang="pug">
  div#about
    h2 About
    img#icon(alt="Vue logo" src="../assets/2896.jpg")
    div#introduction
      div
        h3#name @tocomi
        p スワローズを愛するWebエンジニアです。
        p 競馬は穴党です。
      Sns.section
      div.section
        h2 Skill
        p Java Ruby Rails Python JavaScript Vue.js ReactNative jQuery html pug css sass Delphi COBOL shell
        p EC2 cloudformation lambda firebase Jenkins Ansible Docker Oracle PostgreSQL
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Sns from '../components/Sns.vue'

@Component({
  components: {
    Sns,
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
    .section {
      margin: 50px 0 0 0;
    }
  }
  #sns {
    .icon {
      margin: 10px 15px 0 15px;
      height: 75px;
      width: 75px;
    }
  }
}
</style>

