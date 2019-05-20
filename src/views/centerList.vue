<template lang="html">
  <div class="centerList">
    <Card :bordered="false" >
      <Input  placeholder="在“收集箱”中添加任务，按回车键保存" icon="md-stopwatch" v-on:keyup.enter="addTask" />
        <!-- <Icon type="md-stopwatch" slot="extra" size="16"/>
      </input> -->
    </Card>
    <br/>
    <!-- <Card :bordered="false" > -->
      <CellGroup v-for="task in taskList">
        <Cell :title="task.title" :extra="task.createDate" :label="task.tomatoNum">
          <Radio slot="icon"></Radio>
          <Icon type="md-arrow-dropright-circle" slot="icon" size="16"/>
        </Cell>
      </CellGroup>
    <!-- </Card> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      taskList: [
        {
          title: '任务一',
          createDate: '5月15日',
          tomatoNum: '2个番茄'
        },
        {
          title: '任务二',
          createDate: '5月20日',
          tomatoNum: '2个番茄'
        },
        {
          title: '任务三',
          createDate: '5月16日',
          tomatoNum: '2个番茄'
        }
      ]
    }
  },
  methods: {
    addTask () {
      console.log('增加任务');
    }
  }
}
</script>

<style lang="css" scoped>
  .ivu-cell-item .ivu-radio-wrapper {
    margin-right: 0
  }
  .ivu-cell {
    background: #fff;
    margin-bottom: 5px;
    border-radius: 5px;
  }
</style>
