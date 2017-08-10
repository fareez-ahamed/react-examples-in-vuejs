<template>
<div>Seconds Elapsed: {{ secondsElapsed }}</div>
</template>

<script>
export default {
  data () {
    return {
      secondsElapsed: 0
    }
  },

  created () {
    this.interval = setInterval(() => { this.secondsElapsed++ }, 1000)
  },

  beforeDestroy () {
    clearInterval(this.interval)
  }
}
</script>