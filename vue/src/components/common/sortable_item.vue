<script lang="coffee">
import { ElementMixin, HandleDirective } from 'vue-slicksort';

export default
  mixins: [ElementMixin]
  directives: { handle: HandleDirective },
  props:
    item: Object
</script>

<template lang="pug">
v-list-item.sortable-list-item
  slot
</template>

<style lang="sass">
.sortable-list-item
  font-family: Roboto, sans-serif !important

body > .sortable-list-item
  z-index: 999
</style>
