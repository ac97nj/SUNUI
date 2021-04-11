<demo>
基础用法
</demo>

<template>
  <div>
    <GButton>
      默认按钮
    </GButton>
    <GButton theme="button">
      主要按钮
    </GButton>
    <GButton theme="link">
      链接按钮
    </GButton>
    <GButton theme="text">
      文本按钮
    </GButton>
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
  components: { GButton}
};
</script>

<style lang="scss" scoped>

</style>