<template>
  <canvas class="canvas-gauges"></canvas>
</template>

<script>
import { RadialGauge } from 'canvas-gauges'

export default {

  props: {
    value: Number,
    options: {
      type: Object,
      default: () => ({})
    }
  },

  data () {
    return {
      chart: null
    }
  },

  mounted () {
    this.chart = new RadialGauge(Object.assign(this.options, { renderTo: this.$el, value: this.value }))
      .draw()
  },

  beforeDestroy() {
    this.chart.destroy()
  },

  watch: {
    value (val) {
      this.chart.value = val
    }
  }

}
</script>
