<template>
  <q-page>
    <div class="row items-center justify-evenly">
      <img src="~/src/assets/pic.jpg" />
    </div>
    <div class="row items-center justify-evenly">
      <h1> Welcome to my CV </h1>
      {{ name }}
    </div>
  </q-page>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'

@Component({
  //
})
export default class PageIndex extends Vue {
  name = "Sami Pentti"
}
</script>
