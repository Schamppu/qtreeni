<template>
  <div>
    <q-btn flat color="white" :label="buttonName" @click="buttonPressed" />

  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { Prop } from 'vue-property-decorator'
import Component from 'vue-class-component'

@Component({
  //
})
export default class ToolbarButton extends Vue {
  @Prop({required: true})
  buttonName!: string

  @Prop({required: true})
  linkTo!: string

  buttonPressed() {
    if (this.$router.currentRoute.fullPath !== '/contacts') {
      this.$router.push(this.linkTo)
    }
  }

}
</script>

<style scoped>

</style>
