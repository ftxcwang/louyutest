<template>
  	<div class="hello">
	    <el-row>
		  <el-button plain>朴素按钮</el-button>
		  <el-button type="primary" plain>主要按钮</el-button>
		  <el-button type="success" plain>成功按钮</el-button>
		  <el-button type="info" plain>信息按钮</el-button>
		  <el-button type="warning" plain>警告按钮</el-button>
		  <el-button type="danger" plain>危险按钮</el-button>
		</el-row>

		<el-select v-model="value" placeholder="请选择">
		    <el-option
		      v-for="item in options"
		      :key="item.value"
		      :label="item.label"
		      :value="item.value">
		    </el-option>
		</el-select>
	</div>
</template>

<script>
export default {
  name: 'test',
  data () {
    return {
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
        value: ''
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
