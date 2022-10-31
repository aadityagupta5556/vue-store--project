<template>
  <four-tag  @emit-four="GetDataFromFour"></four-tag>

</template>
  
  <script>
  import Four from './Four.vue'
  export default {
    data() {
        return {        
          name:''
        }
    },
    
    components: {
        'four-tag':Four
    },
    methods: {
        GetDataFromFour(xyz) {
            this.name=xyz
            this.$emit("emit-two",this.name)

        },
        
    }
  }
  </script>
  
  <style>
  
  </style>
  