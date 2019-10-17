<template>
  <div>
    <!-- <el-container class="app-wrapper" id="test">
      <el-header>
        <Header></Header>
      </el-header>
      <el-main>Main</el-main>
      <el-footer>Footer</el-footer>
    </el-container>-->

    <el-container>
      <el-header class="header-wrapper">Header</el-header>
      <el-main>Main</el-main>
      <el-footer>Footer</el-footer>
    </el-container>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";

export default {
  name: "app",
  components: {
    Header
  }
};
</script>

<style lang="scss">
// .app-wrapper {
//   max-width: 1530px;
//   overflow: hidden;
//   margin: 0 auto;
//   .el-header,
//   .el-footer {
//     padding: 0 15px;
//     // background-color: #b3c0d1;
//     color: #333;
//     // text-align: center;
//     line-height: 60px;
//   }
//   .el-main {
//     // &::parent {
//     //   max-width: 100% !important;
//     //   width: 100% !important;
//     // }
//     #test {
//       max-width: 100% !important;
//       width: 100% !important;
//     }
//     padding: 0 15px;
//     background-color: #e9eef3;
//     color: #333;
//     // text-align: center;
//     line-height: 160px;
//   }
// }

.header-wrapper {
   max-width: 1530px;
  overflow: hidden;
  margin: 0 auto;
}

.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 200px;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
