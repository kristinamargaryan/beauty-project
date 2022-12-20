<template>
      <div class="home-header">
      <div class="home-header-left-side">
        <p class="quote"> A whole 
          <span class="motserrat-style"><i>new world</i></span> , a whole <span class="motserrat-style"><i>new look</i></span> </p>
        <p class="quote-text"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin lobortis sed sapien in pretium. Donec tincidunt, quam vestibulum. </p>
        <button class="more-info">
          <span class="more-info-btn">
            DISCOVER MORE
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
      <div class="home-header-carousel">
        <p>carousel</p>
      </div>
    </div>
</template>

<script>
export default {
name:'HomeHeader'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@300&family=Montserrat:wght@100&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@300&family=Montserrat:wght@100&display=swap');
  .home-header{
    display: flex;
    justify-content: space-between;
    height: 880px;
    background: #469597;
    padding:  86px 350px 173px;
  }
  .home-header-left-side{
    margin-top: 35px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    max-width: 667px;
  }
  .quote{
    font-family: 'Cormorant';
    font-style: normal;
    font-weight: 400;
    font-size: 95px;
    line-height: 106px;
    color: #FFFFFF;
    text-align: left;
  }
  .quote-text{
    text-align: left;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 170.02%;
    color: #FFFFFF;
    margin-top: 58px;
  }
  .more-info {
    width: 270px !important;
    min-height: 66px !important;
    background: #FFFFFF;
    border-radius: 60px;
    border: none;
    margin-top: 76px;
  }
  .more-info-btn{
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 170.02%;
    color: #469597;
  }
  .motserrat-style{
    font-family: 'Montserrat';
  }
</style>
