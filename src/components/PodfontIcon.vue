<template>
  <div v-if="svg" v-html="svg" :style="cssProps" :class="size"></div>
</template>

<script>
import PocketCasts from '../podfont-plugin/a-pocket-casts'
export default {
  props: {
    color: {
      type: String,
      default: '#00274c'
    },
    icon: {},
    size: {
      type: String,
      default: 'md'
    }
  },
  data () {
    return {
      svg: PocketCasts
    }
  },
  computed: {
    cssProps () {
      return {
        '--fill-color': this.color
      }
    }
  }
}
</script>

<style scoped lang="scss">
div {
  color: var(--fill-color);
  .xxs {
    width: 0.85em;
  }
  .xs {
    width: 1em;
  }
  .sm {
    width: 1.5em;
  }
  .md {
    width: 2em;
  }
  .lg {
    width: 3em;
  }
  .xl {
    width: 4em;
  }
}
</style>
