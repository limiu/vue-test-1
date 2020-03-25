<template>
  <div>
    <div>n 的zhi为{{n}}</div>
    <div class="row">
      <Cell @click="onClickCell" v-bind:n = "n"/>
      <Cell @click="onClickCell" v-bind:n = "n"/>
      <Cell @click="onClickCell" v-bind:n = "n"/>
    </div>
     <div class="row">
      <Cell @click="onClickCell" v-bind:n = "n"/>
      <Cell @click="onClickCell" v-bind:n = "n"/>
      <Cell @click="onClickCell" v-bind:n = "n"/>
    </div>
     <div class="row">
      <Cell @click="onClickCell" v-bind:n = "n"/>
      <Cell @click="onClickCell" v-bind:n = "n"/>
      <Cell @click="onClickCell" v-bind:n = "n"/>
    </div>
  </div>
</template>

<script>
import Cell from "./Cell";
export default {
  components: { Cell },
  data(){
    return{ n :0};
  },
  methods:{
    onClickCell(){
      console.log("某个Cell被点了")
        this.n += 1;
    }
  }
};

</script>

<style>
.row{
  display: flex;

}
</style>
