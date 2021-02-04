<template>
  <div id="app">
    <div id="tab-bar">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style  scoped>
@import "../../assets/css/base.css";
#tab-bar
{
  display: flex;
  justify-content: space-around;
  background-color: #f6f6f6;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
}


</style>
