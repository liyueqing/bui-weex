<template>
    <div>
        <bui-header
                :title="'布局'"
                :leftItem="leftItem"
                @leftClick="back">
        </bui-header>

        <bui-content-scroll class="span1" padded="true">
            <div>
                <text>flex-direction: row | 从左到右排列.</text>
                <text>flex-direction: column | 从上到下排列.</text>
                <div>
                    <bui-tip type="info" value="flex值1~12. 弹性盒子布局"></bui-tip>
                    <div class="flex-row b-p5" style="align-items: stretch;justify-content: flex-start; height: 100px;">
                        <div class="span1 c-y-f">1</div>
                        <div class="span2 c-b-d">2</div>
                        <div class="span3 c-g-d">3</div>
                        <div class="span4 c-r-f">4</div>
                        <div class="span5 c-b-d">5</div>
                        <div class="span6 c-r-f">6</div>
                        <div class="span7 c-b-d">7</div>
                        <div class="span8 c-r-f">8</div>
                        <div class="span9 c-b-d">9</div>
                        <div class="span10 c-r-f">10</div>
                        <div class="span11 c-b-d">11</div>
                        <div class="span12 c-y-f">12</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="align-items: flex-start; 是上对齐，所有的成员项排列在容器顶部."></bui-tip>
                    <div class="flex-row b-p5" style="align-items: flex-start; height: 500px;">
                        <div class="span6 c-y-f" style="height: 400px;">span1</div>
                        <div class="span3 c-b-d" style="height: 190px;">span2</div>
                        <div class="span3 c-g-d" style="height: 300px;">span3</div>
                        <div class="span5 c-r-f" style="height: 490px;">span4</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="align-items: flex-end; 是下对齐，所有的成员项排列在容器底部."></bui-tip>
                    <div class="flex-row b-p5" style="align-items: flex-end; height: 500px;">
                        <div class="span6 c-y-f" style="height: 400px;">span1</div>
                        <div class="span3 c-b-d" style="height: 190px;">span2</div>
                        <div class="span3 c-g-d" style="height: 300px;">span3</div>
                        <div class="span5 c-r-f" style="height: 490px;">span4</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="align-items: center; 是中间对齐，所有成员项都垂直居中显示."></bui-tip>
                    <div class="flex-row b-p5" style="align-items: center; height: 500px;">
                        <div class="span6 c-y-f" style="height: 400px;">span1</div>
                        <div class="span3 c-b-d" style="height: 190px;">span2</div>
                        <div class="span3 c-g-d" style="height: 300px;">span3</div>
                        <div class="span5 c-r-f" style="height: 490px;">span4</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="align-items: stretch; 是默认值，即拉伸高度至 flex 容器的大小."></bui-tip>
                    <div class="flex-row b-p5" style="align-items: stretch; height: 500px;">
                        <div class="span6 c-y-f">span1</div>
                        <div class="span3 c-b-d">span2</div>
                        <div class="span3 c-g-d">span3</div>
                        <div class="span5 c-r-f">span4</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="justify-content: flex-start; 是默认值，所有的 flex 成员项都排列在容器的前部."></bui-tip>
                    <div class="flex-row b-p5" style="justify-content: flex-start;align-items: stretch; height: 100px;">
                        <div class="c-y-f" style="width:100px">span1</div>
                        <div class="c-b-d" style="width:100px">span2</div>
                        <div class="c-g-d" style="width:150px">span3</div>
                        <div class="c-r-f" style="width:100px">span4</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="justify-content: flex-end; 是意味着成员项排列在容器的后部."></bui-tip>
                    <div class="flex-row b-p5" style="justify-content: flex-end;align-items: stretch; height: 100px;">
                        <div class="c-y-f" style="width:100px">span1</div>
                        <div class="c-b-d" style="width:100px">span2</div>
                        <div class="c-g-d" style="width:150px">span3</div>
                        <div class="c-r-f" style="width:100px">span4</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="justify-content: center; 是中间对齐，成员项排列在容器中间、两边留白."></bui-tip>
                    <div class="flex-row b-p5" style="justify-content: center; align-items: stretch; height: 100px;">
                        <div class="c-y-f" style="width:100px">span1</div>
                        <div class="c-b-d" style="width:100px">span2</div>
                        <div class="c-g-d" style="width:150px">span3</div>
                        <div class="c-r-f" style="width:100px">span4</div>
                    </div>
                </div>

                <div style="margin-top: 30px">
                    <bui-tip type="info" value="justify-content: space-between; 是两端对齐，空白均匀地填充到 flex 成员项之间."></bui-tip>
                    <div class="flex-row b-p5" style="justify-content: space-between; height: 100px;">
                        <div class="c-y-f" style="width:100px">span1</div>
                        <div class="c-b-d" style="width:100px">span2</div>
                        <div class="c-g-d" style="width:150px">span3</div>
                        <div class="c-r-f" style="width:100px">span4</div>
                    </div>
                </div>


                <div style="margin-top:30px">
                    <bui-tip type="info" value="网格布局."></bui-tip>
                    <div v-for="(v, i) in list" class="flex-row" style="height: 80px;">
                        <div v-for="(text, k) in v" class="center span1"
                             style="border-width: 1px;border-color: #d7dde4">
                            <div>
                                <text>{{text}}</text>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </bui-content-scroll>

    </div>
</template>
<style src="../../css/layout.css"></style>
<style src="../../css/header.css"></style>
<style src="../../css/example.css"></style>

<script>
    var buiweex = require("../../js/buiweex.js");
    export default {
        data: function () {
            return {
                leftItem: {
                    icons: 'icon-back',
                },
                list: [
                    ['A', 'B', 'C'],
                    ['D', 'E', 'F'],
                    ['G', 'H', 'I']
                ]
            }
        },
        components: {
            'bui-tip': require('../../components/bui-tip.vue')
        },
        methods: {
            "back": function () {
                buiweex.pop();
            }
        }
    }
</script>