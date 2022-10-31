<template>
  <div>
      <two-tag @emit-two="GetDataFromTwo"></two-tag>
      <three-tag :sendToThree="data"></three-tag>
  </div>

  
</template>

<script>

import Two from './components/Two.vue'
import Three from './components/Three.vue'

export default {
  data() {
    return {
       data:''
    }
  },
  components:{

    'two-tag':Two,
    'three-tag':Three

  },
  methods: {
    GetDataFromTwo(xy) {
     this.data = xy
    },

  }
}
</script>

<style>

</style>