<template>
  
    <div class="thank-you-view">
       <div class="cunstomer-info">
        <img 
        src="../assets/images/img3.svg" 
        class="thank-you-img"
        alt="ThankYou" />
        <h4 class="cunstomer-title">Thank you for your order!</h4>
        <p class="cunstomer-text">Your order is confirmed</p>
        <router-link to="/">
        <button class="cunstomer-button">
            <text class="back-button">Back to Shop</text>
            <img src="../assets/icons/ArrowL.svg" alt="Arrow" class="ArrowL" />
        </button>
        </router-link>
        <div class="box-cunstomer-info">
         <p>Name:
            <span>Oleo Bone</span>
        </p> 
         <hr>
         <p>Email:  
        <span>oleo_bone@gmail.com </span>
        </p>
         <hr>
         <p>Ship to:
        <span>4140 Parker Rd. Allentown, New Mexico 31134</span>
        </p>
         <hr>
        <p>Bill to:
        <span>4140 Parker Rd. Allentown, New Mexico 31134</span></p>
        <hr>
        <p>Payment :
        <span>Credit Card</span></p>
        </div>
           </div>
           <div class="container-summary2">

<h4 class="title10">Order Summary</h4>
    <span>
<img src="../assets/images/img2.svg" alt="no img" class="sho-img" />
    </span>
    <span class="num-summary">1</span>
<span>
  <p class="sho-name">Nike sneakers</p>
  <p class="sho-price">€69.00</p>
</span>

<div class="subtota2">
  <span>
    <p class="subtotal-text">Subtotal</p>
    <p class="subtotal-price">€69.00</p>
  </span>
  <span>
  <p class="subtotal-text2">Shipping</p>
  <p class="subtotal-price2">--</p>
  </span>
  <span>
  <p class="subtotal-text3">Discount</p>
  <p class="subtotal-price3">--</p>
  </span>
  <hr class="line" />
  <span>
  <p class="subtotal-text4">Total</p>
  <p class="subtotal-price4">€69.00</p>
  </span>
</div>
<div class="box-payment2">
  <img 
  src="../assets/icons/fi-rr-lock.svg" 
  alt="lock-img" 
  class="lock-img"
  />
  <p 
  class="secure-pyment">
  Secure SSL Encryption & Guaranteed Safe Checkout
  </p>

  <img 
  src="../assets/icons/payment.svg" 
  alt="credit-icon"
  class="credit-icon"
  />
</div>
</div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.thank-you-view {
    display: flex;
    width: 1920px;
    height: 1055px;
    margin: 0;
    padding-top: 10px;
    background-color: var(--background-primary-page);
    
} 

.thank-you-view ::before {
    content: "";
    opacity: 60%;
    
}

.cunstomer-info {
    position: var(--position-root-absolute);
    width: 972px;
    height: 815px;
    left: 160px;
    top:140px;
    bottom: 100px;
    right: 785px;
    background: var(--background-color-Wite);
    border-radius: 16px;
}
.thank-you-img {
    position: var(--position-root-absolute);
    /* width: 167.07px;
    height: 166.43px; */
    margin-left: 408.89px;
    margin-top: 73.57px;
    margin-bottom: 575px;
    right: 399.04px;
}

.cunstomer-title {
    position: var(--position-root-absolute);
    width: 299px;
    height: 34px;
    left: 338px;
    right: 338px;
    top: 274px;
    bottom: 507px;
    font-family: var(--font-family-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight600);
    font-size: var(--font-size23);
    line-height: var(--line-height34);
    text-align: center;
    color: var(--color-text-primary);

}

.cunstomer-text {
    position: var(--position-root-absolute);
    width: 189px;
    height: 26px;
    left: 393px;
    right: 338px;
    top: 318px;
    bottom: 463px;
    font-family: var(--font-family-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight500);
    font-size: var(--font-size16);
    line-height: var(--line-height26);
    text-align: center;
    color: var(--color-text-secondary);
}

.cunstomer-button {
    position: var(--position-root-absolute);
    width: 213px;
    height: 56px;
    top: 379px;
    bottom: 380px;
    background-color: var(--color-text-primary);
    border-radius: 16px;
    cursor: pointer;
    text-align: center;
    margin-left: 386px;
    margin-top: 20px;
    margin-bottom: 20px;
    right: 386px;
}

.back-button{
    width: 106px;
    height: 20px;
    left: 386px;
    right: 386px;
    top: 379px;
    bottom: 380px;
    font-family: var(--font-family-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight600);
    font-size: var(--font-size16);
    line-height: var(--line-height20);
    color: #FFFFFF;
    text-decoration: none;
}

.ArrowL {
position: var(--position-root-absolute);
left: 13%;
right: 16.67%;
top: 30%;
}

.box-cunstomer-info {
    position: absolute;
    width: 540px;
    height: 280px;
    left: 218px;
    top: 480px;
    background: rgba(239, 240, 245, 0.4);

    border-radius: 16px;
}

.box-cunstomer-info p {
    margin-left: 40px;
    margin-top: 20px;
    margin-bottom: 0px;
    font-family: var(--font-family-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight400);
    font-size: var(--font-size14);
    line-height: var(--line-height24);
    color: var(--color-text-secondary);
}
.box-cunstomer-info hr {
    width: 460px;
    left: 218px;
    top: 480px;
    border: 0.5px solid  rgba(214, 216, 234, 1)
}


.box-cunstomer-info p span {
    width: 302px;
    margin-left: 65px;
    margin-top: 20px;
    margin-bottom: 0px;


    font-family: var(--font-family-Poppins);
    font-style: var(--font-style-normal);
    font-weight: var(--font-weight500);
    font-size: var(--font-size14);
    line-height: var(--line-height24);
    color: rgba(0, 0, 52, 1);

}

.container-summary2 {
    position: var(--position-root-absolute);
  width: 595px;
  height: 388px;
  background: #FFFFFF;
  border-radius: 16px;
  left: 1165px;
  top: 140px;
  right: 160px;
  bottom: 30px;
}

.subtota2 {
    position: var(--position-root-absolute);
    top: 194px;
    left: 40px;


}

.box-payment2{

position: var(--position-root-absolute);
width: 595px;
height: 145px;
left: 0px;
top: 420px;

/* white */

background: var(--background-color-Wite);
border-radius: var(--border-radius-16px);
}



</style>