<template>
  <div class="glassmaterial">
    <div class="inner-shadow"/>
    {{this.msg}}
  </div>
</template>

<script>
export default {
  name: 'glassmaterial',
  props: ['msg']
}
</script>

<style>
.glassmaterial {
  display: flex;
  position: absolute;
  align-content:center;
  align-items: center;
  top:30%;
  left:30%;
  /* background: rgb(248, 248, 252); */
  /* background: rgba(91, 91, 190, 0.8); */
  background: linear-gradient(to right, hsla(240, 63%, 60%, 0.7) 0%, hsla(240, 63%, 55%, 0.6) 100%);
  width: 300px;
  height: 300px;
  border-radius: 15px;
  box-shadow: 5px 5px 15px #2d2d554d;
  color:white;
  filter: blur(0.5px);
  font-size: 32px;
  text-shadow: 2px 2px 1px rgba(20,20, 20,0.2);
  /* box-shadow: 10px 5px 15px rgba(44,44,44,0.3); */
}
.inner-shadow {
  position: absolute;
  top:10px;
  left:10px;
  border-radius: 15px;
  background: rgba(91, 91, 190,0.2);
  box-shadow: 5px 5px rgba(45, 45, 85,0.3);
  /* box-shadow: inset 3px 5px 15px rgba(255,255,255,0.2); */
  /* background: rgba(66,66,66,0.11); */
  filter: blur(2px);
  width: 300px;
  height: 300px;
}
</style>
