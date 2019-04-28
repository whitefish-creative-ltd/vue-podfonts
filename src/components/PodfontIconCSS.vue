<template>
  <i class="pf" :class="classProps"></i>
</template>

<script>
export default {
  props: {
    color: {
      type: String,
      default: '#00274c'
    },
    icon: {
      type: String
    },
    size: {
      type: String,
      default: '1x'
    },
    app: Boolean,
    host: Boolean
  },
  computed: {
    type () {
      return this.host ? 'h' : 'a'
    },
    styleProps () {
      return {
        '--fill-color': this.color
      }
    },
    classProps () {
      return [
        `pf-${this.size}`,
        `pf-${this.type}-${this.icon}`
      ]
    }
  }
}
</script>
