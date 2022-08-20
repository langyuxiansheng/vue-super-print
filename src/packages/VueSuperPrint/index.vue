<!--
 * @Author: zhouliujun
 * @Date: 2022-08-20 20:10:09
 * @LastEditTime: 2022-08-20 21:34:47
 * @LastEditors: zhouliujun
 * @Description: file content
 * @FilePath: /vue-super-print/src/packages/VueSuperPrint/index.vue
 * 可以输入预定的版权声明、个性签名、空行等
-->
<template>
    <div class="app-super-print">
        <div class="app-ctrl-list" remark="组件列表">
            组件列表
        </div>
        <div class="app-print-container" remark="主容器">
            <div class="app-print-tools" remark="工具栏">
                工具栏
            </div>
            <div class="app-print-papers" remark="纸张列表">
                <!-- <div class="app-print-plan"> -->
                    <div class="app-print-paper">
                        <div class="app-paper-content">
                            a4
                        </div>
                        <div class="app-rul-wrapper">
                            <img class="h-img" src="@/assets/rul.png" />
                            <img class="v-img" src="@/assets/rul.png" />
                        </div>
                    </div>
                <!-- </div> -->
            </div>
        </div>
        <div class="app-print-attrs" remark="属性设置">
            属性设置
        </div>
    </div>
</template>
    
<script setup lang='ts'>
</script>
    
<style lang="scss" scoped>
@import "./index.scss";
</style>