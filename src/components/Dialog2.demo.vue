<demo>
一键打开 Dialog
</demo>

<template>
  <div>
    <GButton @click="showDialog">toggle</GButton>
  </div>
</template>

<script lang="ts">
import GDialog from '../lib/GDialog.vue';
import GButton from '../lib/GButton.vue';
import {openDialog} from '../lib/openDialog';
//用户请勿使用上一句
//import { GButton , GDialog ,openDialog } from "sun-hui-0.0.1";
//用户请使用这一句,代替上一句引入文件

//import  "sun-hui-0.0.1/dist/lib/sun-hui-1.css"
// 请用户一定使用这一句, 加上样式


import {h} from 'vue';
export default {
  name: 'Diglog1Demo',
  components: {GButton, GDialog},
  setup() {
    const showDialog = () => {
      openDialog({
        title: h('strong', {}, '标题'),
        content: '你好',
        ok() {
          console.log('ok');
        },
        cancel() {
          console.log('cancel');
        }
      });
    };
    return {showDialog};
  }
};


</script>

<style lang="scss" scoped>

</style>