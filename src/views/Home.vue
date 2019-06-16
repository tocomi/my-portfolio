<template lang="pug">
  div#home
    img(alt="Vue logo" src="../assets/logo.png")
    div#introduction
      h3 @tocomi
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  components: {
  },
})
export default class Home extends Vue {}
</script>
