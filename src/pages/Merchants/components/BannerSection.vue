<template>
    <div class="banner">
        <div class="container">
            <div class="banner-items">
                <h1>Find JuanCash Merchants</h1>
                <g-image src="~/assets/images/merchant/img-header-merchants.png"></g-image>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.banner {
    height: 246px;
    background: url("~@/assets/images/merchant/bg-inner-merchants-top.jpg");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    
    .container {
        .banner-items {
            width: 1000px;
            margin: 0 auto;
            padding-top: 20px;
            h1 {
                float: left;
                position: relative;
                top: 100px;
                left: 100px;
            }

            img {
                position: relative;
            }
        }
    }
}
</style>