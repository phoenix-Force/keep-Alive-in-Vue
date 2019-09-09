<template>
<div>
  <button @click="increase">Increase</button>
  <h2>{{count}}</h2>
</div>

</template>
<script>
export default {
  data:()=>{
    return{
      count:0
    }
  },
  methods:{
    increase(){
      return (this.count ++)
    }
  }

}
</script>
<style scoped>

</style>
