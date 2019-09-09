<template>
  <div id="main" class ="container">
    <div class ="row">
      <div class ="col-xs-12">
        <button class="bg-danger" @click="x='new'"> Load New</button>
        <button class="bg-primary" @click ="x ='App'">Load Default</button>

        <component :is="x">

        </component>

      </div>

    </div>

  </div>


</template>

<script>
import quote from "../src/components/Quote.vue"
import nm from "../src/components/new.vue"
export default {
  components:{
    quoteContent :quote
  },
  data:()=>{
    x:"App"
  }

}
</script>

<style>
h2{
  color:black;
  font-weight: bolder;
  font-size:50px;
  text-align: left;
  margin-top:0px;
}
p{
  color:black;
  font-size:30px;
  text-align: left;
  padding-left:10%;

}

</style>
