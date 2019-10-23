<template>
    <div class="banner-section">
        <div class="container banner-wrapper">
            <p>Boost your business by diversifying your payment options via our latest QR technology</p>
            <g-image src="~/assets/images/business/JuanwithPhone.png"></g-image>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.banner-section {
    .banner-wrapper {        
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        padding: 0 100px;

        p {
            padding-top: 75px;
            width: 572px;
            height: 157px;  
            font-size: 34px;
            font-weight: 600;
            line-height: 1.35;
        }

        img {
            z-index: -1;
        }
    }
}
</style>