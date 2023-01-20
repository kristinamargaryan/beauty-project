<template>
  <div class="our-services">
    <div>
      <p class="our-services-title">
        Get the latest update about our products and services
      </p>
    </div>
    <div class="our-services-form">
      <input class="our-services-input" type="text" placeholder="Your Email" />
      <button class="our-services-btn">SUBSCRIBE</button>
    </div>
  </div>
</template>
<style>
.our-services {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 569px;
  padding: 105px 325px;
  background: #469597;
}
.our-services-title {
  width: 1269px;
  height: 192px;
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 400;
  font-size: 76px;
  line-height: 126.52%;
  text-align: center;
  color: #ffffff;
}
.our-services-form {
  display: flex;
  align-items: center;
  justify-content: space-around;
  border: 2px solid #ffffff;
  width: 751px;
  height: 80px;
  border-radius: 100px;
}
.our-services-input {
  width: 70%;
  border: none !important;
  background: #469597;
  color: #ffffff;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 170.02%;
}
.our-services-input:focus {
  outline: none !important;
}
.our-services-btn {
  background: #ffffff;
  width: 198px;
  height: 63px;
  border-radius: 60px;
  border: none;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 170.02%;
  color: #469597;
}
.our-services-btn:hover {
  background: #e0ecec;
}
input {
  border: none !important;
  box-shadow: none !important;
}
</style>
