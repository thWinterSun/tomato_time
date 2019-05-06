<template lang="html">
  <div class="">
    <Card :bordered="false" >
      <p slot="title">
        <Radio ></Radio>
        <Icon type="ios-arrow-dropright" />
        <!-- <Icon type="ios-play-outline" /> -->
        任务名称
      </p>

      <Icon type="ios-flag-outline" slot="extra" />
      <ul>
        <li>
          <div>
            <Icon type="md-stopwatch" />
            <span>
              番茄数
            </span>
          </div>
        </li>
        <li>
          <div>
            <Icon type="ios-calendar-outline" />
            <span>
              到期日
            </span>
          </div>
        </li>
        <li>
          <div>
            <Icon type="ios-list" />
            <span>
              清单
            </span>
          </div>
        </li>
        <li>
          <div>
            <Icon type="ios-notifications-outline" />
            <span>
              提醒
            </span>
          </div>
        </li>
        <li>
          <div>
            <Icon type="ios-repeat" />
            <span>
              重复
            </span>
          </div>
        </li>
      </ul>
    </Card>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="css">
</style>
