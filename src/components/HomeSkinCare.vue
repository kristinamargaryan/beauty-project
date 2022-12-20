<template>
    <div class="skinCare">
        <div class="skinCare-imgs">
            aaaaaaaaaaaaaaa
            <!-- <img src="@/assets/images/Skin-careimg1.svg" class="skinCare-img1"/>
            <img src="@/assets/images/Skin-careimg2.svg" class="skinCare-img1"/> -->
        </div>
        <div class="skinCare-content">
            <div style="max-width: 604px">
                <img src="@/assets/SkinCare-title.svg" alt="img">
                <p class="skinCare-content-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin lobortis sed sapien in pretium. Donec tincidunt, quam vestibulum ultri</p>
            </div>
            
            
            <!-- it is supposed to change the text in the picture to a list -->
            <div class="skinCare-content-second">
                <img style=" width: 220px" src="@/assets/images/list.svg" alt="list">
                <button class="skin-care-btn">
                   <span >
                       LEARN MORE 
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
        
        </div>
    </div>
</template>
<style>
.skinCare {
    height: 1224px;
    background: #E5E3E4;
    padding: 200px 206px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.skinCare-imgs{
    width:55%;
}
.skinCare-content{
    text-align: left;
    
    display: flex;
    flex-direction: column;
}
.skinCare-content-text{
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 170.02%;
    color: #DDBEAA;
}
.skinCare-content-second {
    display: flex;
    flex-direction: column;
}
.skin-care-btn {
    width: 237px;
    height: 66px;
    background: #469597;
    border-radius: 60px;
    margin: 53px 0;
    border: none;
    color: #E5E3E4;
}

</style>