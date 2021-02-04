<template>
  <div class="tab-bar-item" @click="itemClick">
    <div v-if="!isActive">
      <slot name="item-icon"></slot>
    </div>
    <div v-else>
       <slot  name="item-active-icon"></slot>
    </div>
    <div :style="activeStyle" :class="{active:isActive}">
       <slot name="item-text"></slot>
    </div>
  </div>
</template>


<script>
export default {
    name:"TabBaritem",
    data() {
      return {
        // isActive:false
      }
    },
    computed:{
       isActive()
       {
         return this.$route.path.indexOf(this.path)!=-1
       },
       activeStyle(){
         return this.isActive?{color:this.activecolor}:{}
       }
    },
    props:{
       path:String,
       activecolor:{
         type:String,
         default:'red'
       }
    },
    methods: {
     itemClick()
    {
     this.$router.replace(this.path);
    }
    },
}
</script>

 <style  scoped>
.tab-bar-item
{
  height: 49px;
  text-align: center;
}
.tab-bar-item img{
  height: 24px;
  width: 24px;
}



 </style>
