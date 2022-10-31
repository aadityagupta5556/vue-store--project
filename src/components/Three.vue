<template>
  <seven-tag :sendToSeven="threename"></seven-tag>
</template>

<script>

import Seven from './Seven.vue'
export default {
  data() {
      return {
          threename:''
      }
  },
  props: ['sendToThree'],
  watch: {
    sendToThree(value) {
      this.threename=value
    }
  },
  methods: {
     
    
     },
   mounted () {
    console.log(this.sendToThree, "Three.vue")
   },
  components: {
      'seven-tag':Seven
  },
}
</script>

<style>

</style>