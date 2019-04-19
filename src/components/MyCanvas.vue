<template lang="pug">
  canvas(class="canvas")

</template>

<script>
export default {
  props: {
    radius: {
      type: Number,
      default: 50,
    }
  },
  watch: {
  },
  methods: {
    // Dummy obj
    draw(radius) {
      this.ctx.arc(150, 150, radius, 0, Math.PI * 2)
      this.ctx.fillStyle = 'orange'
      this.ctx.fill()
    }
  },
  // Dummy obj
  mounted() {
    this.ctx = this.$el.getContext('2d')
    this.draw(this.radius)
  }
}
</script>

<style lang="sass" scoped>
.canvas
  width: auto
  height: auto
  margin: 0 auto
  // background-color: rgba(255, 255, 255, .2)
</style>
