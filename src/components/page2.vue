<template lang="pug">
.container
  //------ if need Back -------
  //- .back_org
    .back_mol
      .back_atm
        router-link(to='/') Back

  MyCanvas( :width="width" :height="height")

</template>

<script>
import MyCanvas from './MyCanvas.vue'
export default {
  components: {
    MyCanvas
  },
  data() {
    return {
      // width: 300,
      // height: 200,
    }
  }
}
</script>

<style lang="sass" scoped>
.back
  &_org
    position: absolute
    top: 20px
    left: 20px
  &_mol
    background: darkorange
    border-radius: 10px
    box-shadow: 0px 4px 0 #222
    border: 2px solid #fff

  &_atm
    a
      display: block
      padding: .35em 1.5em
      text-decoration: none
      color: white
      font-size: 1.3em
      font-weight: 600

.container
  background: linear-gradient(-45deg, rgba(29,93,35,.9), rgba(95,95,228,.8))
  width: 100%
  height: 100%
  min-height: 100vh
  padding: 0
</style>
