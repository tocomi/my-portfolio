<template lang="pug">
  div#about
    h2 About
    img#icon(alt="Vue logo" src="../assets/2896.jpg")
    div#introduction
      div.section
        h3#name @tocomi
        p スワローズを愛するWebエンジニアです。
        p 競馬は穴党です。
      hr.separator
      Sns.section
      hr.separator
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
  margin: auto;
  max-width: 700px;
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
      margin: 30px 0;
    }
    .separator {
      border: 0;
      border-top: 1px solid #DADADA;
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

