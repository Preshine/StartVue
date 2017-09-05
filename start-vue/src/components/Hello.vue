<template>
  <div class="hello" v-show="showHello" ref="hello">
    <el-row>
      <el-col :span="8"  class="logo" ><span>Preshine'Vue</span></el-col><el-col :span="16" class="avator" ><img src="./logo.jpg"  /><div class="user"><span>{{username}}</span>,欢迎登陆!</div></el-col>
    </el-row>
    <el-row class="tac">
      <el-col :span="4">
        <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose">
          <el-submenu index="1">
            <template slot="title">
              <i class="el-icon-message"></i>基础对象</template>
            <el-menu-item-group>
              <template slot="title">分组一</template>
              <el-menu-item index="1-1">仓库</el-menu-item>
              <el-menu-item index="1-2">客户</el-menu-item>
            </el-menu-item-group>
            <el-menu-item-group title="分组2">
              <el-menu-item index="1-3">资金</el-menu-item>
            </el-menu-item-group>
            <el-submenu index="1-4">
              <template slot="title">供应商</template>
              <el-menu-item index="1-4-1">销售</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-menu-item index="2">
            <i class="el-icon-menu"></i>业务应用</el-menu-item>
          <el-menu-item index="3">
            <i class="el-icon-setting"></i>科目表表</el-menu-item>
        </el-menu>
      </el-col>
      <el-col :span="20">
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data() {
    return {
      username: 'Preshine',
      showHello: true
    }
  },
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.logo {
  line-height: 80px;
  font-size: 40px;
  background: #d1dbe5;
}
.avator {
  height: 80px;
  background: #d1dbe5;
}
.avator .user {
  line-height: 70px;
  height: 70px;
  float: right;
}
.avator span {
  color: red;
}
.avator img {
  height: 50px;
  margin: 8px;
  border-radius: 50%;
  float: right;
  padding: 8;
}
.avator img:hover {
  cursor: pointer;
}
</style>
