<template lang="pug">
div
  canvas(class="canvas")

  .toggle(v-on:click='isActive=!isActive') Canvas hide

  section.content_lay.d-none(v-bind:class="{ active: isActive }")
    .content_inner
      .org_inner
        .mol_inner
          .atom_inner
            .mock Content

</template>

<script>
export default {
  data() {
    return {
      // Canvas hide = false
      isActive: true,
    }
  },
  props: {
  },
}
</script>

<style lang="sass" scoped>
.toggle
  position: absolute
  right: 20px
  top: 20px
  background: #eee
  padding: 10px 20px
  cursor: pointer

.d-none
  &.active
    display: none

.mock
  margin-top: 40px
  font-size: 1.5em

.canvas
  width: 100vw
  height: 100%
  min-height: 100vh
  margin: 0 auto
  background-color: rgba(255, 155, 0, .9)
  // background-color: rgba(0, 0, 0, .5)

section.content_lay
  position: absolute
  left: 0
  top: 0
  -webkit-transform: translate(-50%, -50%)
  transform: translate(0%, 0%)
  right: 0
  bottom: 0
  width: 100vw
  min-height: 100vh
  background: aliceblue
</style>
