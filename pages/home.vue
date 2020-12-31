<template>
    <div class="home">
        <HeaderLogo/>
        <HeaderMenu>
            <div class="region" slot="region">
                <i class="el-icon-menu"></i>
                区域中心
                </div>
        </HeaderMenu>
        <div class="container">
            <div class="sideCarouselLogin">
                <div class="side"></div>
                <div class="carousel"></div>
                <div class="login"></div>
            </div>
        </div>
    </div>
</template>
<style lang="less" scoped>
.home{
    width: 100%;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    background-color: #f6f6f6;
    .container{
        width: 1200px;
        .region{
            background-color: #f6f6f6;
            padding: 11px 15px;
        }
    }
}
</style>