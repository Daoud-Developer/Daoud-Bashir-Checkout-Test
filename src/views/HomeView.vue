<template>
  <div class="container">
    <img class="home-img" src="../assets/images/img1.svg" alt="Vue logo" />
    <icon class="Epllise-Right">
      <img src="../assets/icons/Fi-angle-right.svg" class="Fi-angle-right" />
    </icon>
    <icon class="Epllise-Left">
      <img src="../assets/icons/Fi-angle-left.svg" class="Fi-angle-left" />
    </icon>
    <img />
  <div class="text">
    <span class="textPrice">Price:</span>
    <span class="text50">$50</span>

    <div class="text80">
      <span class="num80">-80%</span>
    </div>

    <div class="quntity">
      <span class="Quantity1">Quantity:</span>
      <icon class="bg-minus">
        <img src="../assets/icons/Fi-minus.svg" class="Fi-minus" />
      </icon>
      <span class="num1">1</span>
      <icon class="bg-plus">
        <img src="../assets/icons/Fi-plus.svg" class="Fi-plus" />
      </icon>
    </div>
  </div>
  <div class="textDescription">
    <p class="textDescription1">
    Ornare rhoncus nunc ut felis. Faucibus dolor at ultrices tincidunt. Pulvinar sed justo et 
    viverra pellentesque.
    </p>
    <p class="textDescription2">
    Mauris augue nulla proin vel a. Facilisis fringilla molestie dignissim elit orci malesuada.
    Lorem sit sagittis vitae nulla id. Mauris ipsum sed sed faucibus. Nulla amet metus
    gravida orci faucibus nisl eros arcu lorem. Nullam ornare molestie nam id gravida 
    volutpat bibendum sem feugiat. Neque vulputate in et maecenas porta mi tellus.In 
    massa porttitor urna quis volutpat at.
    </p>
  </div>
  <div class="box1">

    <icon class="icon-lock">
        <img src="../assets/icons/lock.svg" class="Fi-shopping-cart" />
        
    </icon>
    <span class="text-lock">Guaranteed <strong> Safe </strong> & <strong>Secure</strong> Checkout</span>

    <icon class="icon-payment">
        <img src="../assets/icons/payment.svg" class="Fi-shopping-cart" />
    </icon>

  </div>
    <div class="box-support">
        <icon class="icon-shopping-cart">
            <img src="../assets/icons/support.svg"  class="Fi-support" />
        </icon>
        <span class="text-support"><strong>24/7</strong><br/>Support</span>
    </div>
     <router-link to="/checkout" >
        <button  class="btn-shopping">
           <text class="text-shopping">Yes, I want <img src="../assets/icons/ArrowR.svg" class="ArrowR" /></text>
        </button>
      </router-link>
           <router-link to="#" class="link-shopping">No, Thanks </router-link>
  </div>
</template>
<script>
export default {
  name: "HomeViews",
  components: {

  },
};
</script>


<style> 
.container {
width: 1920px;
height: 1584px;
left: 0px;
top: 0px;

/* Background */
background:var(--background-primary-page);
  }

  /* .container::before {
  content: "";
  opacity: 0.6;
} */
  
  .home-img {
    position: var(--position-root-absolute);
    width: 790px;
    height: 520px;
    left: 565px;
    top: 140px;
  }
  
  /* Ellipse 314 */
  .Epllise-Right {
    box-sizing: var(--box-sizing-border-box);
  
    position: var(--position-root-absolute);
    width: 44px;
    height: 44px;
    left: 595px;
    top: 378px;
    border-radius: 50%;
    /* white */
    border: 1px solid var(--background-color-Wite);
  }
  
  .Fi-angle-right {
    position: var(--position-root-absolute);
    left: 25%;
    right: 25%;
    top: 25%;
    bottom: 0%;
  }
  
  /* Ellipse 314 */
  .Epllise-Left {
    position: var(--position-root-absolute);
    width: 44px;
    height: 44px;
    left: 1281px;
    top: 378px;
    border-radius: 50%;
  
    /* white */
    background: var(--background-color-Wite);
    opacity: 0.5;
  }
  
  .Fi-angle-left {
    position: var(--position-root-absolute);
    left: 40%;
    right: 25%;
    top: 25%;
    bottom: 0%;
  }
  
  .text {
    position: var(--position-root-absolute);
    width: 790px;
    height: 225px;
    left: 565px;
    right: 565px;
    top: 690px;
    bottom: 690px;
    border-radius: 16px;
    /* white */
    background: var(--background-color-Wite);
    border: 1px solid #daddf5;
    box-shadow: 0px 10px 30px rgba(22, 8, 49, 0.05);
  }
  
  /* Price: */
  .textPrice {
    position: var(--position-root-absolute);
    width: 55px;
    height: 30px;
    left: 285px;
    right: 450px;
    top: 45px;
    bottom: 150px;
    margin: 0px 0px 0px 10px;
    font-family: var(--font-primary-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight500);
    font-size: var(--font-size20);
    line-height: var(--line-height30);
    color: var(--color-text-primary);
  }
  
  /* $50 */
  .text50 {
    position: var(--position-root-absolute);
    left: 350px;
    right: 381px;
    top: 40px;
    bottom: 145px;
    /* font */
    font-family: var(--font-primary-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight600);
    font-size: var(--font-size30);
    line-height: var(--line-height40);
    color: var(--color-text-primary);
  }
  
  /* -80% */
  .text80 {
    position: var(--position-root-absolute);
    width: 84px;
    height: 36px;
    left: 421px;
    right: 285px;
    margin-right: 12px;
    top: 42px;
    bottom: 147px;

    /* color */
    background: var(--background-color-lte1);
    border-radius: 8px;
  }
  
  .num80 {
    position: var(--position-root-absolute);
    width: 54px;
    height: 30px;
    top: 3px;
    left: 15px;
    right: 15px;
    bottom: 3px;
    font-family: var(--font-primary-Poppins);
    font-style: var(--font-style-normal);
    font-weight:var(--font-weight500);
    font-size: var(--font-size20);
    line-height: var(--line-height30);
    color: var(--color-text-primary);
  }
  
  .quntity {
    position: var(--position-root-absolute);
    width: 540px;
    height: 80px;
    left: 125px;
    right: 125px;
    top: 105px;
    bottom: 40px;
  
    /* Color*/
    background: #eff0f5;
    border-radius: var(--border-radius-16px);
  }
  
  .Quantity1 {
    position: absolute;
    width: 92px;
    height: 30px;
    left: 114px;
    right: 334px;
    top: 25px;
    bottom: 25px;
    /* font */
    font-family: var(--font-primary-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight500);
    font-size: var(--font-size20);
    line-height: var(--line-height30);
  
    /* color */
    color: var(--color-text-secondary);
  }
  
  .bg-minus {
    position: var(--position-root-absolute);
    width: 57px;
    height: 50px;
    top: 15px;
    left: 245px;
    right: 238px;
    bottom: 15px;
    cursor: pointer;
    /* Color*/
    background: var(--background-color-Wite);
    border-radius: var(--border-radius-16px);
  }
  .Fi-minus {
    width: 20px;
    height: 1.67px;
    position: absolute;
    left: 19px;
    right: 18px;
    top: 24.17px;
    bottom: 24.17px;
    
  
    /* color */
  
    background: var(--color-text-primary);
  }
  
  .num1 {
    position: var(--position-root-absolute);
    width: 8px;
    height: 30px;
    left: 332px;
    right: 200px;
    top: 25px;
    bottom: 35px;

  /* font */
    font-family: var(--font-primary-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight600);
    font-size: var(--font-size20);
    line-height: var(--line-height30);

    /* color */
    color: var(--color-text-primary);
  }
  
  .bg-plus {
    position: var(--position-root-absolute);
    width: 57px;
    height: 50px;
    left: 370px;
    right: 113px;
    top: 15px;
    bottom: 15px;
    cursor: pointer;
    /* color */
    background: var(--background-color-Wite);
    border-radius: var(--border-radius-16px);
  }
  
  .Fi-plus {
    position: var(--position-root-absolute);
    left: 19px;
    right: 18px;
    top: 15px;
    bottom: 15px;
  }
  /* fix this */
  .textDescription {
    position: var(--position-root-absolute);
    width: 790px;
    height: 208px;
    left: 565px;
    top: 955px;
    /* font */
    font-family: var(--font-primary-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight400);
    font-size: var(--font-size16);
    line-height: var(--line-height26);
    /* color */
    color: var(--color-text-secondary);
  }
  
  .box1 {
  box-sizing: var(--box-sizing-border-box);
  position: var(--position-root-absolute);
  width: 475px;
  height: 140px;
  left: 565px;
  right: 880px;
  top: 1223px;
  bottom: 405px;
  margin-bottom: 40px;
  
  /* color */
  
  background: var(--background-color-Wite);
  border: 1px solid #DADDF5;
  box-shadow: 0px 10px 30px rgba(22, 8, 49, 0.05);
  border-radius: var(--border-radius-16px);
  }
  
  .icon-lock {
    position: var(--position-root-absolute);
    left: 73px;
    right: 382px;
    top: 31px;
    bottom: 85px;
  }
  
  .text-lock {
    position: var(--position-root-absolute);
    width: 295px;
    height: 26px;
    left: 110px;
    right: 70px;
    top: 30px;
    bottom: 84px;
   /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
  color: var(--color-text-secondary);
  }
  
  .icon-payment {
    position: var(--position-root-absolute);
    left: 71px;
    right: 89px;
    top: 86px;
    bottom: 30px;
  }
  
  .box-support {
    position: var(--position-root-absolute);
    box-sizing: var(--box-sizing-border-box);
    width: 285px;
    height: 140px;
    left: 1070px;
    right: 565px;
    top: 1223px;
    bottom: 405px;
    margin-bottom: 40px;
  
  /* white */
  background: var(--background-color-Wite);
  border: 1px solid #DADDF5;
  box-shadow: 0px 10px 30px rgba(22, 8, 49, 0.05);
  border-radius: var(--border-radius-16px);
  }
  
  .Fi-support {
    position: var(--position-root-absolute);
    left: 56.55px;
    right: 165.55px;
    top: 35px;
    bottom: 35px;
  }
  
  .text-support {
  position: var(--position-root-absolute);
  width: 80px;
  height: 60px;
  left: 153px;
  right: 52px;
  top: 42px;
  bottom: 38px;
  color: var(--color-text-primary);
  padding: 0;
   /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-size: var(--font-size20);
  line-height: var(--line-height30);
  }
  
  .btn-shopping {
  position: var(--position-root-absolute);
  width: 281.29px;
  height: 76.43px;
  left: 819px;
  right: 819.71px;
  top: 1433px;
  bottom: 258.57px;
  cursor: pointer;
  /* Background */
  color: var(--background-color-Wite);

  background: #050824;
  border-radius: 135.714px;
  
  }
  
  .text-shopping {
  position: var(--position-root-absolute);
  width: 132px;
  height: 33px;
  left: 54.29px;
  right: 95px;
  top: 21.71px;
  bottom: 21.71px;
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size24);
  line-height: var(--line-height33);
  text-decoration: none;
  color: var(--background-color-Wite);
  }
  
  .ArrowR{
  position: var(--position-root-absolute);
  left: 100%;
  right: 0%;
  top: 22.05%;
  bottom: 22.05%;
  }
  
  .link-shopping {
      position: var(--position-root-absolute);
  width: 101px;
  height: 24px;
  left: 909px;
  top: 1540px;
  
  text-decoration: none;
  
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size18);
  line-height: var(--line-height24);
  
  /* color */
  
  color: var(--color-text-secondary);
  }
  
</style>
