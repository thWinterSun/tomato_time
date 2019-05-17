<template lang="html">
  <div class="">
    <Card :bordered="false" >
      <Input  placeholder="在“收集箱”中添加任务，按回车键保存" icon="md-stopwatch"/>
    </Card>
    <br/>
    <Card :bordered="false" >
      <CellGroup>
        <Cell title="任务1" extra="5月15日" >

        </Cell>
        <Cell title="任务2" extra="5月16日" >

        </Cell>
        <Cell title="任务3" extra="5月15日" >
          
        </Cell>
      </CellGroup>
    </Card>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="css">
</style>
