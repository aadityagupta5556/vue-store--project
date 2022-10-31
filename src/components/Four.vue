<template>
    <div>
        <h1 @click="SendToTwo">button</h1>
    </div>
</template>
  
<script>


export default {

    data() {
        return {

        }
    },
    mounted() {
        this.$emit('emit-four', 'mobiotics')

    },

    methods: {
        SendToTwo() {
            this.$emit('emit-four', 'mobiotics company')
        }
    },

}
</script>
  
<style>

*{
    margin: 0;
    padding: 0;

}


</style>
  