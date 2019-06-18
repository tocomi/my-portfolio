<template lang="pug">
  div#about
    h2 About
    img#icon(alt="Vue logo" src="../assets/2896.jpg")
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

<style lang="scss" scoped>
#about {
  #icon {
    border-radius: 50%;
    height: 150px;
    width: 150px;
  }
}
</style>

