<template>
  <div class="headerLogo">
    <div class="container">
      <div>logo</div>
      <div class="searchBox">
          <el-input placeholder="请输入搜索内容" v-model="searchWord" clearable />
          <el-button  icon="el-icon-search" ></el-button>
      </div>
      <div class="buyCar">
        <el-badge :value="12" class="item">
          <el-button icon="el-icon-shopping-cart-1">我的购物车</el-button>
        </el-badge>
      </div>
    </div>
  </div>
</template>
<script>
export default {
    data(){
        return{
            searchWord:undefined
        }
    }
}
</script>
<style lang="less" scoped>
.headerLogo {
    width: 100%;
  height: 70px;
  display: flex;
  justify-content: center;
  background-color: #fff;
  .container{
      width: 1200px;
      padding: 0 100px 0 0;
      display: flex;
      justify-content: space-between;
      align-items: center;
      .searchBox {
          display: flex;
          margin-right: -200px;
          .el-input{
              /deep/ .el-input__inner{
                  border:#bf1b2b 1px solid; 
                  width: 400px;
                  margin-right: -2px;
              }
          }
          .el-button{
              background-color: #bf1b2b;
              color: #fff;
          }
      }
      .buyCar{
          .el-button{
              color: #bf1b2b;
          }
      }
  }
}
</style>