<template>
  <eight-tag :sendToEight="data"></eight-tag>
</template>

<script>

import Eight from './Eight.vue'
export default {
  data() {
      return {
          data:''
      }
  },
  watch: {
      sendToSeven(val) {
        this.data = val
      }
  },
  props: ['sendToSeven'],
  methods: {
     
    
     },
  
  components: {
      'eight-tag':Eight
  },
}
</script>

<style>

</style>