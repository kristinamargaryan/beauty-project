<template>
  <div class="products">
    <div class="products-about">
        <<h2 class="products-title">Our Product</h2>>
        <p class="products-about-text">Lorem ipsum dolor sit amet, consec tetur adipiscing elit.</p>
        <button class="shop-now-btn">
            <span class="shop-now-btn-name">
                SHOP NOW 
                 <svg xmlns="http://www.w3.org/2000/svg"
                      width="16" 
                      height="16" 
                      fill="currentColor" 
                      class="bi bi-arrow-right" 
                      viewBox="0 0 16 16">
                    <path fill-rule="evenodd" 
                          d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"/>
                  </svg> 
            </span>
        </button>
    </div>
    <div class="img-carousel"></div>
  </div>
</template>

<script>
export default {
name: 'ProductsShortPage'
}
</script>

<style>
.products{
    background-color: #5BA199;
    height: 720px;
    padding: 0 148px;
    display: flex;
    align-items: center;
}
.products-about{
    width: 35%;
    text-align: left;
}
.products-title{
    font-family: 'Cormorant';
    font-style: normal;
    font-weight: 400;
    font-size: 76px;
    line-height: 126.52%;
    color: #FFFFFF;
    text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    margin-bottom: 20px;
}
.products-about-text{
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 170.02%;
    color: #FFFFFF;
    margin-bottom: 42px;
}
.shop-now-btn{
    width: 226px;
    height: 66px;
    border-radius: 60px;
    border:none;
}
.shop-now-btn-name{
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 170.02%;
    text-align: right;
    color: #469597;
}
</style>