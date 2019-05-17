<template lang="html">
  <div class="">
    <Card :bordered="false" >
      <p slot="title">
        <Radio ></Radio>
        <!-- <Icon type="ios-arrow-dropright" /> -->
        <!-- <Icon type="ios-play-outline" /> -->
        任务名称
      </p>

      <Icon type="ios-flag-outline" slot="extra" size='25'/>

      <CellGroup>
        <Cell title="番茄数" extra="5月15日" >
          <Icon type="md-stopwatch" slot="icon" size='20'/>
        </Cell>
        <Cell title="到期日" extra="5月16日 周四" >
          <Icon type="ios-calendar-outline" slot="icon" size='20'/>
        </Cell>

        <Cell title="清单" extra="收集箱" >
          <Icon type="ios-list" slot="icon" size='22'/>
        </Cell>
        <Cell title="提醒" extra="无" >
          <Icon type="ios-notifications-outline" slot="icon" size='20'/>
        </Cell>
        <Cell title="重复" extra="无" >
          <Icon type="ios-repeat" slot="icon" size='20'/>
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
