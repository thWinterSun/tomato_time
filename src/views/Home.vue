<style lang="less" scoped>
.layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
}


.ivu-layout-sider{
  background: #fff;
  .ivu-menu-item{
    .ivu-icon{
      font-size: 18px
    }
  }
}

.ivu-layout-header{
  background: #fff;
  height: 50px;
  line-height: 50px;
  border-bottom: 1px solid #ddd;
  box-shadow: 0 2px 6px rgba(0,0,0,.2);
  .login {
    span{
      color:red;
    }
  }
  .avatar .ivu-icon,.info .ivu-icon{
    font-size: 25px;
    margin-right: 10px;
    color: #ccc;
  }
}


.ivu-menu-vertical .ivu-menu-item{
  padding: 5px 0;
}
</style>
<template>
    <div class="layout">
        <Layout>
            <Header>
              <Row>
                <Col span="4">
                  <span class="avatar">

                    <Icon type="md-contact" />
                  </span>
                  <span class="login">
                    登陆
                  </span>
                  |
                  <span>
                    注册
                  </span>
                </Col>
                <Col span="3" offset="17">
                  <div class="info">
                    <span>
                      <Icon type="ios-stats-outline" />
                    </span>
                    <span>
                      <Icon type="ios-notifications-outline" />
                    </span>
                    <span>
                      <Icon type="ios-settings-outline" />
                    </span>
                  </div>
                </Col>

              </Row>
            </Header>
            <Layout>
              <Sider >
                <Menu active-name="1-2" theme="light" width="auto" >
                  <CellGroup>
                    <MenuItem name="1-1">
                        <Cell title="今天" extra="1.7h" >
                          <Icon type="md-sunny" slot="icon" />
                        </Cell>
                    </MenuItem>
                    <MenuItem name="1-2">
                        <Cell title="明天" extra="0h" >
                          <Icon type="ios-partly-sunny" slot="icon" />
                        </Cell>
                    </MenuItem>
                    <MenuItem name="1-3">
                        <Cell title="待定" extra="1.8h" >
                          <Icon type="md-calendar" slot="icon" />
                        </Cell>
                    </MenuItem>
                    <MenuItem name="1-4">
                        <Cell title="即将到来" extra="0h" >
                          <Icon type="md-calendar" slot="icon" />
                        </Cell>
                    </MenuItem>
                  </CellGroup>
                </Menu>
              </Sider>
                <Layout :style="{padding: '24px 24px'}">

                    <Content :style="{ minHeight: '280px'}">
                      <Row :gutter="20">
                        <Col span="16">
                          <Total></Total>
                          <br />
                          <List></List>
                        </Col>
                        <Col span="8">
                          <Right></Right>
                        </Col>
                      </Row>
                    </Content>
                </Layout>
            </Layout>
        </Layout>
    </div>
</template>
<script>
  import Total from '@/views/centerTotal.vue'
  import List from '@/views/centerList.vue'
  import Right from '@/views/rightMenu.vue'

  export default {
    components: {
      Total,
      List,
      Right
    }
  }
</script>
