<!--
 * @Author: zhouliujun
 * @Date: 2022-08-19 09:41:50
 * @LastEditTime: 2022-08-20 20:38:51
 * @LastEditors: zhouliujun
 * @Description: file content
 * @FilePath: /vue-super-print/src/App.vue
 * 可以输入预定的版权声明、个性签名、空行等
-->
<template>
    <VueSuperPrint />
</template>
<script lang="ts">
import { defineComponent, reactive } from "vue";
// import { VisualEditor } from "../src/packages/visual-editor";
// import { TestUseModel } from "../src/packages/utils/useModel";
// import visualConfig from "./packages/visual.config";
import VueSuperPrint from "./packages/index";
export default defineComponent({
    name: "App",
    components: { VueSuperPrint },
    setup() {
        const jsonData = reactive({
            container: {
                height: 500,
                width: 800
            },
            blocks: [
                {
                    componentKey: "button",
                    top: 100,
                    left: 100,
                    focus: false,
                    width: 0,
                    height: 0,
                    adjustPosition: true,
                    props: {}
                },
                {
                    componentKey: "input",
                    top: 200,
                    left: 200,
                    focus: false,
                    width: 0,
                    height: 0,
                    adjustPosition: true,
                    props: {}
                }
            ]
        });

        return {
            jsonData
            // visualConfig
        };
    }

    // data() {
    //     return {
    //         visualConfig,
    //         jsonData:
    //     };
    // }
});
</script>