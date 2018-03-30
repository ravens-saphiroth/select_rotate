<template>
  <section>
    <el-select v-model="value" @visible-change="handle" class="select-list" popper-class="option-list" placeholder="请选择">
      <el-option
        v-for="item in options"
        :key="item.value"
        :label="item.label"
        :value="item.value">
      </el-option>
    </el-select>
    <el-popover
      ref="popover"
      placement="top-start"
      title="标题"
      width="200"
      trigger="click"
      content="这是一段内容,这是一段内容,这是一段内容,这是一段内容。">
    </el-popover>
    <el-button v-popover:popover>click 激活</el-button>
  </section>
</template>

<script>
  export default {
    data () {
      return {
        value: '',
        options: [{
          value: '选项1',
          label: '黄金糕'
        }, {
          value: '选项2',
          label: '双皮奶'
        }, {
          value: '选项3',
          label: '蚵仔煎'
        }, {
          value: '选项4',
          label: '龙须面'
        }, {
          value: '选项5',
          label: '北京烤鸭'
        }],
        rangeValue: 10
      }
    },
    methods: {
      handle(visible) {
        let docEl = document.querySelector('.select-list')
        console.log(docEl, docEl.getBoundingClientRect())
      },
    }
  }
</script>