<template>
    <div class="headerMenu">
        <div class="container">
            <div class="containerLeft">
                <slot name="region"></slot>
        <nuxt-link :to="{name:'home'}" >主页</nuxt-link>
       <nuxt-link :to="{name:'stock'}" >现货市场</nuxt-link>
       <nuxt-link :to="{name:'futures'}" >期货市场</nuxt-link>
       <nuxt-link :to="{name:'news'}" >资讯中心</nuxt-link>
       <nuxt-link :to="{name:'aboutUs'}" >关于我们</nuxt-link>
            </div>
        </div>
    </div>
</template>
<style lang="less" scoped>
.headerMenu{
  width: 100%;
  height: 46px;
  display: flex;
  justify-content: center;
  background-color: #fff;
  .container{
      width: 1200px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      .containerLeft{
          width: 600px;
          display: flex;
          justify-content: space-between;
          align-items: center;
      }
  }
}
</style>