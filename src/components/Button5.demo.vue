<demo>
加载按钮
</demo>


<template>
  <div>
    <GButton loading>加载中</GButton>
    <GButton>加载完毕</GButton>
  </div>
</template>

<script lang="ts">
import GButton from '../lib/GButton.vue';
//用户请勿使用上一句
//import { GButton  } from "sun-hui-0.0.1";
//用户请使用这一句,代替上一句引入文件

//import  "sun-hui-0.0.1/dist/lib/sun-hui-1.css"
// 请用户一定使用这一句, 加上样式



export default {
  components: {GButton}
};
</script>

<style lang="scss" scoped>

</style>