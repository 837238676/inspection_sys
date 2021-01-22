<template>
    <div>
        <div class="about">
            <h1>This is an about page</h1>
        </div>
        <vue-okr-tree :data="testData"/>
    </div>
</template>

<script>
    import {VueOkrTree} from 'vue-okr-tree';
    import 'vue-okr-tree/dist/vue-okr-tree.css'

    export default {
        name: '',
        components: {
            VueOkrTree
        },
        data() {
            return {
                testData: [{
                    label: 'xxx科技有有限公司',
                    children: [{
                        label: '产品研发部',
                        children: [{
                            label: '研发-前端',
                        }, {
                            label: '研发-后端',
                        }, {
                            label: 'UI 设计',
                        }]
                    }, {
                        label: '销售部',
                        children: [{
                            label: '销售一部',
                        }, {
                            label: '销售二部',
                        }
                        ]
                    }, {
                        label: '财务部'
                    }]
                }]
            }
        }
    }
</script>
