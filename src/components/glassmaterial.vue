<template>
  <div class="glassmaterial" v-bind:style="{width:size, height:size}">
    <div class="inner-shadow" v-bind:style="{width:size, height:size, left:depth, top:depth}">
    </div>
    <div class="outer-shadow" v-bind:style="{width:size, height:size, left:depth, top:depth}"/>
    {{this.msg}}
  </div>
</template>

<script>
export default {
  name: 'glassmaterial',
  props: ['msg', 'size', 'depth']
}
</script>

<style>
.glassmaterial {
  padding: 10px;
  display: flex;
  margin: 30px;
  /* position: absolute; */
  align-content:center;
  align-items: center;
  top:30%;
  left:30%;
  /* background: rgb(248, 248, 252); */
  /* background: hsla(240, 63%, 55%, 0.1); */
  background: linear-gradient(to right, hsla(240, 63%, 60%, 0.4) 0%, hsla(240, 63%, 55%, 0.4) 100%);
  width: 300px;
  height: 100px;
  border-radius: 15px;
  box-shadow: 5px 5px 10px hsla(240, 63%, 55%, 0.2);
  color:white;
  filter: blur(0.5px);
  font-size: 32px;
  text-shadow: 2px 2px 1px rgba(20,20, 20,0.2);
  /* box-shadow: 10px 5px 15px hsla(240,63,55,0.2); */
}
.inner-shadow {
  position: absolute;
  padding: 10px;
  top:10px;
  left:10px;
  border-radius: 15px;
  /* background: rgba(91, 91, 190,0.05); */
  background: linear-gradient(to right, hsla(240, 63%, 60%, 0.1) 0%, hsla(240, 63%, 55%, 0.1) 100%);
  /* box-shadow: inset 3px 5px 15px rgba(255,255,255,0.2); */
  /* background: rgba(66,66,66,0.11); */
  filter: blur(2px);
  width: 300px;
  height: 100px;
}
.outer-shadow{
  position: absolute;
  padding: 10px;
  top:10px;
  left:10px;
  border-radius: 15px;
  /* box-shadow: 5px 5px rgba(45, 45, 85,0.2); */
  box-shadow: 5px 5px hsla(240, 63%, 55%, 0.2);
  filter: blur(3px);
  width: 300px;
  height: 100px;
}
</style>
