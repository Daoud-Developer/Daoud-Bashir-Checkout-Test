<template>
  <div class="checkout-page">
    <div class="container1">
      <div class="hero">
        <span class="title1">Checkout</span>
        <p class="title2">
          Strong demand! Complete your order before it's too late!
        </p>
      </div>
      <div class="container2">
        <p class="title3">Your cart is reserved for 10:00 minutes.</p>
      </div>
      <div class="container3">
        <h5 class="title4">Express Checkout</h5>
        <icon class="icon-shopPay">
          <img
            class="iconpay1"
            src="../assets/icons/shopPay.svg"
            alt="shopPay"
          />
        </icon>
        <icon class="icon-paypal">
          <img class="iconpay2" src="../assets/icons/paypal.svg" alt="visa" />
        </icon>
        <icon class="icon-googlepay">
          <img class="iconpay3" src="../assets/icons/googlepay.svg" alt="" />
        </icon>
      </div>
      <div class="container4">
        <h5 class="title5">Lifetime Warranty🔥</h5>
        <p class="title6">
          Add a lifetime warranty & enjoy peace of mind for life with your dream
          collections order for just $4.99
        </p>
        <button class="btn-warranty">
          <text class="btn-text1">Add- $4.99</text>
        </button>
      </div>
      <div class="container5">
        <h4 class="title7">Contact information</h4>
      </div>

      <form class="contact-form">
        <input  
        class="inputemail"
         type="email" 
        v-model="email"
         placeholder="Email Address" 
         required />
        <img src="../assets/icons/email.svg" alt="fi-email" class="fi-email" />
        <br />
        <input class="inputphone" type="tel" placeholder="Phone Number" />
        <img src="../assets/icons/tel.svg" alt="fi-phone" class="fi-phone" />
        <br />
        <input
          class="inputsingup"
          type="checkbox"
          id="vehicle1"
          name="vehicle1"
          value="Bike"
        />
        <label class="label-signup" for="vehicle1"
          >Sign up for exclusive offers and news
        </label>
        <br />
        <h4 class="title8">Shipping address</h4>
        <div class="Shipping address">
          <input
            class="inputcountry"
            type="select"
            placeholder="Select a Country"
          />
          <img
            src="../assets/icons/fi-rr-location-alt.svg"
            alt="location"
            class="fi-location"
          />
          <img
            src="../assets/icons/fi-sr-angle-down.svg"
            alt="angle-down"
            class="angle-down"
          />
          <br />

          <img
            class="fi-user"
            src="../assets/icons/fi-rr-user.svg"
            alt="fi-user"
          />
          <input
            type="text"
            id="fname"
            icon="fi-rr-user"
            class="inputfname"
            placeholder="First Name"
          />

          <input
            placeholder="Last Name"
            class="inputlname"
            type="text"
            id="lname"
          />
          <img
            class="fi-user1"
            src="../assets/icons/fi-rr-user.svg"
            alt="fi-user"
          />
          <br />
          <input class="inputaddress" type="text" placeholder="Address" />
          <img
            src="../assets/icons/fi-rr-home.svg"
            alt="fi-rr-home"
            class="fi-rr-home"
          />
          <br />
          <input
            class="inputbuilding"
            type="text"
            placeholder="Aparment, suit, etc (Optional)"
          />
          <img
            src="../assets/icons/fi-rr-building.svg"
            alt="fi-rr-building"
            class="fi-rr-building"
          />
          <br />
          <input
            type="text"
            id="city"
            icon="fi-rr-user"
            class="input-city"
            placeholder="City"
          />

          <input
            placeholder="Post code"
            class="input-postcode"
            type="text"
            id="postcode"
            name="postcode"
          />
        </div>

        <h4 class="title9">Shipping method</h4>

        <div class="shipping">
          <div class="shipping1">
            <input type="radio" id="free" name="shipping" value="free" />
            <label for="free">Free shipping</label>
          </div>
          <br />
          <div class="shipping2">
            <input type="radio" id="DHL" name="shipping" value="DHL" />
            <label for="DHL">DHL with price</label>
          </div>
        </div>
        <h4 class="billing-addressh4">Billing address</h4>
        <p class="billing-addressp">
          Specify the address for your payment option
        </p>
        <div class="same-billing">
          <input type="radio" id="same" name="billing" value="same" />
          <label for="same">Same as shipping address</label>
        </div>
        <div class="same-billing1">
          <input type="radio" id="different" name="billing" value="different" />
          <label for="different">Use a different billing address</label>
        </div>
      </form>
    </div>

    <div class="container-summary">

      <h4 class="title10">Order Summary</h4>
          <span>
      <img src="../assets/images/img2.svg" alt="no img" class="sho-img" />
          </span>
          <span class="num-summary">1</span>
      <span>
        <p class="sho-name">Nike sneakers</p>
        <p class="sho-price">€69.00</p>
      </span>
      <div class="discount-code">
        <input class="input-discount" type="text" placeholder="Discount code" />
        <button class="btn-discount">
          <text class="btn-text2">Apply</text>
        </button>
      </div>

      <div class="subtotal">
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
      <div class="box-payment">
        <img 
        src="../assets/icons/fi-rr-lock.svg" 
        alt="lock-img" 
        class="lock-img"
        />
        <p 
        class="secure-pyment ">
        Secure SSL Encryption & Guaranteed Safe Checkout
        </p>
      
        <img 
        src="../assets/icons/payment.svg" 
        alt="credit-icon"
        class="credit-icon"
        />
      </div>
      
      <div class="box-text">
       <p class="text1">
        The ultimate jewellery club
      </p>
        <p class="text2">
          Ornare rhoncus nunc ut felis. Faucibus dolor at ultrices tincidunt. Pulvinar sed justo et viverra pellentesque.
        </p>

        <p class="text3">
          <img src="../assets/icons/fi-rr-check.svg" alt="star" class="fi-true" />
          Extra 10$ off!
        </p>

        <p class="text4">
          <img src="../assets/icons/fi-rr-check.svg" alt="star" class="fi-true1" />
          Free shipping on marked club items!
        </p>

        <p class="text5">
          <img src="../assets/icons/fi-rr-check.svg" alt="star" class="fi-true2" />
          Free returns on marked club items!
        </p>
      </div>

      <div class="box-payment1">
        <h4 class="title11">Payment Method</h4>
        <form>
          <div class="payment-method1">
            <input 
            type="radio" 
            id="credit"
            class="credit-card"
             value="credit" />
            <label class="credit1" for="credit">Credit Card</label>
            <img src="../assets/icons/card-viza.svg" alt="credit-icon" class="credit-icon1" />
            <input type="text" placeholder="Card number" class="card-number" />
            <img src="../assets/icons/card.svg" alt="credit-icon" class="card-icon2" />
            <input type="text" placeholder="Name on the card" class="name-card" /> 
            <img src="../assets/icons/fi-rr-user.svg" alt="credit-icon" class="card-icon3" /> 
            <input type="text" placeholder="MM/YY" class="mm-yy" />
            <img src="../assets/icons/data-icon.svg" alt="credit-icon" class="data-icon" />
            <input type="text" placeholder="CVC" class="cvc" />
            <img src="../assets/icons/cvv-lock.svg" alt="credit-icon" class="cvv-lock-icon5" /> 
            
          </div>
          <div class="payment-method2">
            <input type="radio" id="paypal" value="paypal" class="paypal-payment" />
            <label class="text-paypal" for="paypal">PayPal</label>
            <img src="../assets/icons/paypal-2.svg" alt="credit-icon" class="paypal-icon6" />
          </div>

          <div class="box-agree" >
            <input type="checkbox" id="agree" value="agree" class="agree" />
            <label class="agree-text" for="agree">By checking this box, I acknowledge that I have read and agree to the<strong> Terms of Service</strong>, and <strong>Monthly Billing Terms</strong> of this website and 
            want to opt-in for the monthly billed Dream Collection Club®</label>
            <router-link to="/thankyou" >
            <button type="submit" class="btn-pay">
              <text  class="btn-text3">Complete Purchase</text>
            </button>
          </router-link>
          </div>
        </form>
      </div>
    </div>
   

  </div>

</template>

<script>

export default {
  name: "checkout",
  data() {
    return {
      sho: [
        {
          id: 1,
          name: "Nike sneakers",
          price: 69,
          img: "../assets/images/img2.svg",
        },
      ],
    };
  },
};





</script>

<style>
.checkout-page {
  position: var(--position-root-absolute);
  width: 1920px;
  height: 2105px;
  left: 0px;
  right: 0px;
  /* Color& Background*/
  background: var(--background-primary-page);
}

.container1 {
  position: var(--position-root-absolute);
  width: 975px;
  height: 1945px;
  margin-top: 60px;
  margin-left: 160px;
  margin-right: 785px;
  margin-bottom: 100px;
  background: var(--background-color-Wite);
  border-radius: var(--border-radius-16px);
}

.title1 {
  position: var(--position-root-absolute);
  width: 180px;
  height: 46px;
  margin-right: 755px;
  margin-left: 40px;
  margin-top: 40px;
  bottom: 1859px;

  /* Headline/H2/bold */

  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight700);
  font-size: var(--font-size36);
  line-height: var(--line-height46);
}

.title2 {
  position: var(--position-root-absolute);
  width: 566px;
  height: 30px;
  margin-right: 369px;
  margin-left: 40px;
  margin-top: 50px;
  margin-bottom: 0px;
  bottom: 1779px;
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size20);
  line-height: var(--line-height30);
}

.container2 {
  position: var(--position-root-absolute);
  width: 895px;
  height: 56px;
  margin-right: 40px;
  margin-left: 40px;
  margin-top: 186px;
  margin-bottom: 1703px;

  /* Color& Background*/
  background: var(--background-color-primary);
  border-radius: var(--border-radius-16px);
}

.title3 {
  width: 309px;
  height: 20px;

  /* Space */
  margin: 18px 18px 561px 25px;
  /* Font */

  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);

  /* Color& Background*/
  color: var(--color-text-secondary);
}

.container3 {
  position: var(--position-root-absolute);
  width: 895px;
  height: 160px;
  margin-right: 40px;
  margin-left: 40px;
  margin-top: 272px;
  margin-bottom: 1513px;
  /* Color& Background*/
  background: var(--background-color-Wite);
  border: 1px solid #d6d8ee;
  border-radius: var(--border-radius-16px);
}

.title4 {
  width: 178px;
  height: 30px;
  box-sizing: border-box;
  /* Space */
  margin-top: 30px;
  margin-left: 30px;
  margin-bottom: 100px;
  margin-right: 687px;
  /* Font */

  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size20);
  line-height: var(--line-height30);

  /* Color& Background*/
  color: var(--color-text-primary);
}

.icon-shopPay {
  position: var(--position-root-absolute);
  width: 147px;
  height: 50px;
  top: 80px;
  left: 30px;
  bottom: 30px;
  right: 718px;

  /* color& background */
  background: rgba(90, 49, 244, 0.1);
  border: 1px solid rgba(90, 49, 244, 0.6);
  border-radius: 16px;
}

.iconpay1 {
  position: var(--position-root-absolute);
  width: 84px;
  height: 20px;
  top: 15px;
  left: 31px;
  bottom: 15px;
  right: 32px;
}

.icon-paypal {
  position: var(--position-root-absolute);
  width: 147px;
  height: 50px;
  top: 80px;
  left: 197px;
  bottom: 30px;
  right: 551px;

  /*  color& background */
  background: rgba(17, 57, 132, 0.1);
  border: 1px solid rgba(17, 57, 132, 0.6);
  border-radius: 16px;
}

.iconpay2 {
  position: var(--position-root-absolute);
  width: 82px;
  height: 20px;
  top: 15px;
  left: 33px;
  bottom: 15px;
  right: 32px;
}

.icon-googlepay {
  position: var(--position-root-absolute);
  width: 147px;
  height: 50px;
  top: 80px;
  left: 364px;
  bottom: 30px;
  right: 385px;

  /*  color& background */
  background: rgba(234, 64, 50, 0.1);
  border: 1px solid rgba(234, 64, 50, 0.6);
  border-radius: 16px;
}

.iconpay3 {
  position: var(--position-root-absolute);
  width: 50px;
  height: 20px;
  top: 15px;
  left: 48px;
  bottom: 15px;
  right: 48px;
}

.container4 {
  position: var(--position-root-absolute);
  width: 895px;
  height: 145px;
  margin-right: 40px;
  margin-left: 40px;
  margin-top: 452px;
  margin-bottom: 1348px;

  /* Color& Background*/
  background: rgb(96%, 96%, 97%);
  border-radius: 16px;
}

.title5 {
  width: 199px;
  height: 30px;
  /* Space */
  margin-top: 30px;
  margin-left: 30px;
  margin-bottom: 85px;
  /* margin-right: 666px; */
  /* Font */

  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: 19px;
  line-height: var(--line-height30);

  /* Color& Background*/
  color: var(--color-text-primary);
}

.title6 {
  position: var(--position-root-absolute);
  width: 635px;
  height: 48px;
  top: 67px;
  left: 30px;
  bottom: 30px;
  right: 230px;
  /* Font */

  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size14);
  line-height: var(--line-height24);

  /* Color& Background*/
  color: var(--color-text-secondary);
}

.btn-warranty {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-start;
  padding: 11px 30px;
  gap: 10px;
  /* Space */
  position: absolute;
  width: 115px;
  height: 62px;
  right: 30px;
  top: 42px;
  bottom: 41px;
  left: 750px;
  /* Color& Background*/
  background: #000034;
  border-radius: 10px;
  cursor: pointer;
}

.btn-text1 {
  width: 45px;
  height: 40px;
  top: 11px;
  bottom: 11px;
  left: 35px;
  right: 35px;

  /* Font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
  /* Color& Background*/
  color: white;
}

.container5 {
  position: var(--position-root-absolute);
  width: 895px;
  top: 647px;
  left: 40px;
  bottom: 1364px;
  right: 689px;
}

.title7 {
  position: var(--position-root-absolute);
  width: 246px;
  height: 34px;
  top: -30px;

  /* Font */

  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size24);
  line-height: var(--line-height34);

  /* Color& Background*/
  color: var(--color-text-primary);
}

.contact-form {
  position: var(--position-root-absolute);
  width: 895px;
  left: 40px;
  right: 40px;
  top: 701px;
  bottom: 1364px;
}

.inputemail {
  box-sizing: border-box;
  width: 895px;
  height: 56px;
  text-align: left;
  padding-left: 60px;
  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);

  /* Color& Background*/
  border: 1px solid rgba(214, 216, 238, 1);
  border-radius: 16px;
}

.inputemail:focus {
  outline: none;
  border: 1px solid #000034;
}

.inputemail::placeholder {
  width: 115px;
  height: 20px;
  top: 18px;
  left: 25px;
  bottom: 18px;
  right: 850px;

  /* Color& Background*/
  color: var(--background-color-lte);
}

.fi-email {
  position: var(--position-root-absolute);
  top: 18.83px;
  left: 25px;
  bottom: 18.83px;
  right: 850px;
}

.inputphone {
  box-sizing: border-box;
  width: 895px;
  height: 56px;
  margin: 24px 0;
  padding-left: 60px;
  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);

  /* Color& Background*/
  border: 1px solid rgba(214, 216, 238, 1);
  border-radius: 16px;
}

.inputphone:focus {
  outline: none;
  border: 1px solid #000034;
}

.inputphone::placeholder {
  width: 115px;
  height: 20px;
  top: 18px;
  left: 25px;
  bottom: 18px;
  right: 850px;

  /* Color& Background*/
  color: var(--background-color-lte);
}

.fi-phone {
  position: var(--position-root-absolute);
  top: 100px;
  left: 25px;
  bottom: 100px;
  right: 850px;
}

.inputsingup {
  width: 22px;
  height: 22px;
  top: 26px;
  left: 40px;
  bottom: 52px;
  right: 913px;
  cursor: pointer;
}

input[type="checkbox"] {
  accent-color: var(--color-text-secondary);
}

.label-signup {
  position: var(--position-root-absolute);
  width: 858px;
  height: 26px;
  padding: 0px 0px 0px 15px;
  /* Font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size16);
  line-height: var(--line-height26);

  /* Color& Background*/
  color: var(--color-text-secondary);
}

.title8 {
  width: 212px;
  height: 34px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size24);
  line-height: var(--line-height34);
}

.inputcountry {
  box-sizing: border-box;
  padding-left: 60px;
  width: 895px;
  height: 56px;
  border: 1px solid #d6d8ee;
  border-radius: 16px;
  top: 991px;
  left: 40px;
  bottom: 898px;
  right: 40px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}

.inputcountry::placeholder {
  /* Color& Background*/
  color: var(--background-color-lte);
}

.inputcountry:focus {
  outline: none;
  border: 1px solid var(--color-text-primary);
}

.fi-location {
  position: var(--position-root-absolute);
  top: 306px;
  left: 25px;
  bottom: 18px;
  right: 850px;
}

.angle-down {
  position: var(--position-root-absolute);
  top: 315px;
  left: 850px;
  bottom: 18px;
  right: 25px;
}

.inputfname {
  /* position: var(--position-root-absolute); */
  box-sizing: border-box;
  padding-left: 60px;
  margin-top: 24px;
  width: 436px;
  height: 56px;
  border: 1px solid #d6d8ee;
  border-radius: 16px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}

.inputfname:focus {
  outline: none;
  border: 1px solid var(--color-text-primary);
}

.inputlname {
  position: var(--position-root-absolute);
  box-sizing: border-box;
  padding-left: 60px;
  width: 436px;
  height: 56px;
  border: 1px solid #d6d8ee;
  border-radius: 16px;
  margin: 24px 0;
  left: 460px;
  right: 40px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}

.inputlname:focus {
  outline: none;
  border: 1px solid var(--color-text-primary);
}

.inputfname::placeholder {
  /* Color& Background*/
  color: var(--background-color-lte);
}

.inputlname::placeholder {
  /* Color& Background*/
  color: var(--background-color-lte);
}

.fi-user {
  position: var(--position-root-absolute);
  left: 25px;
  bottom: -406px;
  right: 890px;
}

.fi-user1 {
  position: var(--position-root-absolute);
  left: 480px;
  bottom: -406px;
  right: 890px;
}

.inputaddress {
  /* position: var(--position-root-absolute); */
  box-sizing: border-box;
  padding-left: 60px;
  width: 895px;
  height: 56px;
  border: 1px solid #d6d8ee;
  border-radius: 16px;
  margin-top: 24px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}

.inputaddress:focus {
  outline: none;
  border: 1px solid var(--color-text-primary);
}

.inputaddress::placeholder {
  /* Color& Background*/
  color: var(--background-color-lte);
}

.fi-rr-home {
  position: var(--position-root-absolute);
  left: 25px;
  bottom: -487px;
  right: 890px;
}

.inputbuilding {
  /* position: var(--position-root-absolute); */
  box-sizing: border-box;
  padding-left: 60px;
  width: 895px;
  height: 56px;
  border: 1px solid #d6d8ee;
  border-radius: 16px;
  margin-top: 24px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}

.inputbuilding:focus {
  outline: none;
  border: 1px solid #000034;
}

.inputbuilding::placeholder {
  /* Color& Background*/
  color: var(--background-color-lte);
}

.fi-rr-building {
  position: var(--position-root-absolute);
  left: 25px;
  bottom: -568px;
  right: 890px;
}

.input-city {
  /* position: var(--position-root-absolute); */
  box-sizing: border-box;
  padding-left: 25px;
  width: 436px;
  height: 56px;
  border: 1px solid #d6d8ee;
  border-radius: 16px;
  margin-top: 24px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}

.input-city:focus {
  outline: none;
  border: 1px solid #000034;
}

.input-city::placeholder {
  /* Color& Background*/
  color: var(--background-color-lte);
}

.input-postcode {
  position: var(--position-root-absolute);
  box-sizing: border-box;
  padding-left: 25px;
  width: 436px;
  height: 56px;
  border: 1px solid #d6d8ee;
  border-radius: 16px;
  margin-top: 24px;
  left: 460px;
  right: 40px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}

.input-postcode:focus {
  outline: none;
  border: 1px solid #000034;
}

.input-postcode::placeholder {
  /* Color& Background*/
  color: var(--background-color-lte);
}

.title9 {
  width: 210px;
  height: 34px;
  top: 0px;
  right: 725px;
  bottom: 0px;
  left: 40px;
  margin-top: 50px;

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size24);
  line-height: var(--line-height34);
  color: var(--color-text-primary);
}

.shipping1 {
  width: 895px;
  height: 64px;
  background: rgba(239, 240, 245, 0.4);
  border-radius: 16px;
}
.shipping1 input {
  width: 24px;
  height: 24px;
  margin-top: 20px;
  margin-left: 20px;
  margin-bottom: 20px;
}

.shipping1 input[type="radio"] {
  accent-color: var(--color-text-secondary);
}

.shipping1 label {
  position: var(--position-root-absolute);
  margin-left: 10px;
  margin-top: 20px;
  margin-bottom: 20px;
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height24);
}

.shipping2 {
  width: 895px;
  height: 64px;
  background: rgba(239, 240, 245, 0.4);
  border-radius: 16px;
}
.shipping2 input {
  width: 24px;
  height: 24px;
  margin-top: 24px;
  margin-left: 20px;
  margin-bottom: 20px;
}

.shipping2 input[type="radio"] {
  accent-color: var(--color-text-secondary);
}

.shipping2 label {
  position: var(--position-root-absolute);
  margin-left: 10px;
  margin-top: 20px;
  margin-bottom: 20px;
  color: #4b4e68;
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height24);
}

.billing-addressh4 {
  margin-top: 50px;
  left: 40px;
  right: 758px;
  bottom: 238px;

  /* color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size24);
  line-height: var(--line-height34);
}

.billing-addressp {
  position: var(--position-root-absolute);
  margin-top: -30px;
  width: 312px;
  height: 21px;

  /* color */
  color: var(--color-text-secondary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size14);
  line-height: var(--line-height21);
}

.same-billing {
  width: 895px;
  height: 64px;
  background: rgba(239, 240, 245, 0.4);
  border-radius: 16px;
}

.same-billing input {
  width: 24px;
  height: 24px;
  margin-top: 20px;
  margin-left: 20px;
  margin-bottom: 20px;
}

.same-billing input[type="radio"] {
  accent-color: var(--color-text-secondary);
}

.same-billing label {
  position: var(--position-root-absolute);
  margin-left: 10px;
  margin-top: 20px;
  margin-bottom: 20px;
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height24);
}

.same-billing1 {
  width: 895px;
  height: 64px;
  margin-top: 24px;
  background: rgba(239, 240, 245, 0.4);
  border-radius: 16px;
}

.same-billing1 input {
  width: 24px;
  height: 24px;
  margin-top: 20px;
  margin-left: 20px;
  margin-bottom: 20px;
}

.same-billing1 input[type="radio"] {
  accent-color: var(--color-text-secondary);
}

.same-billing1 label {
  position: var(--position-root-absolute);
  margin-left: 10px;
  margin-top: 20px;
  margin-bottom: 20px;
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height24);
}


/* order summary */

.container-summary {
  position: var(--position-root-absolute);
  width: 595px;
  height: 474px;
  background: #FFFFFF;
  border-radius: 16px;
  left: 1165px;
  top: 60px;
  right: 160px;
  bottom: 30px;
}

.title10 {
  position: var(--position-root-absolute);
  width: 194px;
  height: 34px;
  margin-left: 40px;
  margin-top: 40px;
  margin-right: 361px;
  margin-bottom: 400px;

  /*  color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight500);
font-size: var(--font-size24);
line-height: var(--line-height34);


}

.sho-img {
  position: var(--position-root-absolute);
  width: 55.29px;
  height: 52px;
  margin-left: 40px;
  margin-top: 112px;
  margin-right: 499.71px;
  margin-bottom: 310px;
  border-radius: 8px;
}

.num-summary {
  position: var(--position-root-absolute);
  padding: 0.2rem 0.4rem;
  margin-left: 85px;
  top: 104px;
  margin-right: 492px;
  margin-bottom: 352px;

  /* color */
  color: #fff;

  /* font */
  border-radius: 60%;
  background-color:var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size12);
  line-height: var(--line-height12);
}

.sho-name {
  position: var(--position-root-absolute);
  width: 110px;
  height: 26px;
  margin-left: 115.29px;
  margin-top: 124px;
  margin-right: 369.71px;
  margin-bottom: 324px;

  /* color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.sho-price {
  position: var(--position-root-absolute);
  width: 110px;
  height: 26px;
  /* text-align: right; */
  margin-left: 497px;
  margin-top: 124px;
  margin-right: 40px;
  margin-bottom: 324px;

  /* color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.discount-code {
  position: var(--position-root-absolute);
  margin-left: 40px;
  margin-top: 194px;
  margin-right: 455px;
  margin-bottom: 268px;
}

.discount-code input {
  box-sizing: border-box;
  width: 361px;
  height: 56px;
  padding-left: 25px;
  border: 1.5px solid #EBECF3;
  border-radius: 16px;
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height24);
}

.discount-code input:focus {
  outline: none;
  border: 1.5px solid var(--color-text-secondary);
}

.discount-code input::placeholder {
  color: #84849A;
}

.discount-code button {
  position: var(--position-root-absolute);
  width: 120px;
  height: 56px;
  margin-left: 24px;
  margin-top: 0px;
  margin-right: 40px;
  margin-bottom: 0px;
  background: var(--color-text-primary);
  border-radius: var(--border-radius-16px);
  cursor: pointer;
}

.discount-code button text {
  font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight500);
font-size: var(--font-size16);
line-height: var(--line-height24);
  color: #FFFFFF;
}

.subtotal {
  position: var(--position-root-absolute);
  margin-left: 40px;
  margin-top: 280px;
  margin-right: 487px;
  margin-bottom: 168px;
}

.subtotal-text {
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.subtotal-price {
  width: 110px;
  height: 26px;
  margin-left: 460px;
  margin-top: -41px;

  /* color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.subtotal-text2 {
  /* position: var(--position-root-absolute); */
  margin-left: 0px;
  margin-top: 0px;
  margin-right: 0px;
  margin-bottom: 0px;
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.subtotal-price2 {
  width: 110px;
  height: 26px;
  margin-left: 501px;
  margin-top: -20px;
  margin-right: 40px;
  margin-bottom: 0px;

  /* color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.subtotal-text3 {
  /* position: var(--position-root-absolute); */
  margin-left: 0px;
  margin-top: 15px;
  margin-right: 0px;
  margin-bottom: 0px;
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.subtotal-price3 {
  width: 110px;
  height: 26px;
  margin-left: 501px;
  margin-top: -20px;
  margin-right: 40px;
  margin-bottom: 0px;

  /* color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.line {
  position: var(--position-root-absolute);
  width: 515px;
  margin-left: 0px;
  margin-top: 0px;
  margin-right: 40px;
  margin-bottom: 0px;
  border: 1px solid #EBECF3;
}

.subtotal-text4 {
  /* position: var(--position-root-absolute); */
  margin-left: 0px;
  margin-top: 10px;
  margin-right: 0px;
  margin-bottom: 0px;
  color: var(--color-text-primary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.subtotal-price4 {
  width: 110px;
  height: 26px;
  margin-left: 460px;
  margin-top: -25px;
  margin-right: 40px;
  margin-bottom: 0px;

  /* color */
  color: var(--color-text-primary);

  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size16);
  line-height: var(--line-height26);
}

.box-payment {
  position: absolute;
width: 595px;
height: 145px;
left: 0px;
top: 504px;

/* white */

background: #FFFFFF;
border-radius: 16px;
}


.lock-img {
  position: var(--position-root-absolute);
width: 18px;
height: 18px;
left: 112.25px;
top: 42px;
bottom: 89.5px;
right: 481.25px;
}

.secure-pyment {
  position: var(--position-root-absolute);
width: 400px;
left: 135px;
top: 24px;
right: 100px;

/* font */
font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight400);
font-size: var(--font-size14);
line-height: var(--line-height26);

}

.credit-icon {
  position: var(--position-root-absolute);
  left: 160px;
  top: 81px;
  bottom: 40px;
  right: 160px;

}

.box-text {
  position: var(--position-root-absolute);
  width: 595px;
height: 267px;
left: 0px;
top: 679px;

  /* white */

  background: #FFFFFF;
  border-radius: 16px;
}

.text1 {
  width: 320px;
  margin-left: 40px;
  margin-top: 40px;
  margin-right: 235px;
  margin-bottom: 200px;

  /* color */
  color: var(--color-text-primary);
  /* font */
  font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight600);
font-size: var(--font-size18);
line-height: var(--line-height27);
}

.text2 {

  width: 515px;
  height: 48px;

  margin-left: 40px;
  margin-top: -188px;
  margin-right: 40px;
  margin-bottom: 0px;
  
  /* color */
  color: var(--color-text-secondary);
  /* font */
font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight400);
font-size: var(--font-size14);
line-height: var(--line-height24);
}

.text3 {
  width: 515px;
  height: 48px;

  margin-left: 66px;
  margin-top: 12px;
  margin-right: 40px;
  margin-bottom: 0px;
  
  /* color */
  color: var(--color-text-secondary);
  /* font */
font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight400);
font-size: var(--font-size14);
line-height: var(--line-height24);
}

.text4 {
  width: 255px;
  height: 24px;

  margin-left: 66px;
  margin-top: -15px;
  margin-right: 274px;
  margin-bottom: 0px;
  
  /* color */
  color: var(--color-text-secondary);
  /* font */
font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight400);
font-size: var(--font-size14);
line-height: var(--line-height24);

}

.text5 {
  width: 255px;
  height: 24px;

  margin-left: 66px;
  margin-top: 12px;
  margin-right: 274px;
  margin-bottom: 0px;
  
  /* color */
  color: var(--color-text-secondary);
  /* font */
font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight400);
font-size: var(--font-size14);
line-height: var(--line-height24);
  
  }

  .fi-true {
    position: var(--position-root-absolute);
    left: 40.02px;
    right:538.98px;
    top: 146px;
    bottom: 0px;
  }

  .fi-true1{
    position: var(--position-root-absolute);
    left: 40.02px;
    right:538.98px;
    bottom: 75px;
  }

  .fi-true2{
    position: var(--position-root-absolute);
    left: 40.02px;
    right:538.98px;
    bottom: 40px;
  }

 .box-payment1 {
  position: var(--position-root-absolute);
  width: 595px;
  height: 726px;
  left: 0px;
  top: 976px;
/* white */
background: #FFFFFF;
border-radius: 16px;
 }

 .title11 {
  position: var(--position-root-absolute);
 margin-top: 40px;
 margin-left: 40px;
  /* color */
  color: var(--color-text-primary);
  /* font */
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size24);
  line-height: var(--line-height34);
 }

 .payment-method1{
  position: var(--position-root-absolute);
  width: 515px;
  height: 310px;
  left: 40px;
  top: 104px;
  background: rgba(239, 240, 245, 0.4);
  border-radius: 16px;
 }

 .credit-card{
  position: var(--position-root-absolute);
  width: 24px;
  height: 24px;
  left: 20px;
  top: 20px;
  bottom: 266px;
  right: 471px;
 }

 .credit-card,input[type="radio"] {
  accent-color: var(--color-text-secondary);
}

.credit1 {
  position: var(--position-root-absolute);
  left: 60px;
  top: 25px;
  bottom: 0px;
  right: 0px;
  /* color */
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height24);
}

.credit-icon1 {
  position: absolute;
left: 290px;
right: 20px;
top: 20px;
bottom: 266px;
}

.card-number {
  position: var(--position-root-absolute);
  width: 415px;
  height: 56px;
  margin-left: 20px;
  margin-top: 64px;


  border: 1px solid #D6D8EE;
  border-radius: 16px;  
  /* font */
  font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight500);
font-size: var(--font-size16);
line-height: var(--line-height20);
}

.card-number ,input:focus {
  outline: none;
  border: 1.5px solid var(--color-text-secondary)
}



.card-number input::placeholder {
  color: #979AB8;
}

.card-number,input[type="text"] {
  padding-left: 60px;
}

.card-icon2 {
  position: var(--position-root-absolute);
  left: 45px;
  top: 84.5px;
  bottom: 522.5px;
}

.name-card {
  position: var(--position-root-absolute);
  width: 415px;
  height: 56px;
  margin-left: 20px;
  margin-top: 144px;

  border: 1px solid #D6D8EE;
  border-radius: 16px;  
  /* font */
  font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight500);
font-size: var(--font-size16);
line-height: var(--line-height20);
}

.card-icon3 {
  position: var(--position-root-absolute);
  left: 45px;
  top: 162px;
  bottom: 128px;
  right: 0px;
}

.mm-yy {
  position: var(--position-root-absolute);
  width: 160px;
  padding: 0px;
  height: 56px;
  left: 20px;
  top: 224px;

  border: 1px solid #D6D8EE;
  border-radius: 16px;  
  /* font */
  font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight500);
font-size: var(--font-size16);
line-height: var(--line-height20);
}

.data-icon {
  position: var(--position-root-absolute);
  left: 45px;
  top: 242px;
  bottom: 0px;
  right: 0px;
}

.cvc {
  position: var(--position-root-absolute);
  width: 160px;
  height: 56px;
  margin-left: 270px;
  margin-top: 224px;

  border: 1px solid #D6D8EE;
  border-radius: 16px;  
  /* font */
  font-family: var(--font-primary-Poppins);
font-style: var(--font-style-normal);
font-weight: var(--font-weight500);
font-size: var(--font-size16);
line-height: var(--line-height20);
}

.cvv-lock-icon5 {
  position: var(--position-root-absolute);
  left: 290px;
  top: 242px;
  bottom: 0px;
  right: 0px;
}

.payment-method2 {
  position: var(--position-root-absolute);
  width: 515px;
  height: 64px;
  left: 40px;
  top: 434px;
  background: rgba(239, 240, 245, 0.4);
  border-radius: 16px;
}

.paypal-payment{
  position: var(--position-root-absolute);
  width: 24px;
  height: 24px;
  left: 20px;
  top: 20px;
  bottom: 20px;
}

.text-paypal {
  position: var(--position-root-absolute);
  left: 60px;
  top: 23px;
  bottom: 20px;
  right: 405px;
  /* color */
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight500);
  font-size: var(--font-size16);
  line-height: var(--line-height24);
}

.paypal-icon6 {
  position: var(--position-root-absolute);
  width: 78px;
  height: 24px;
  left: 417px;
  top: 20px;
  bottom: 20px;
  right: 20px;
}

.box-agree {
  position: var(--position-root-absolute);
  width: 483px;
  height: 72px;
  left: 40px;
  top: 528px;
  bottom: 126px;
}

.agree {
  position: var(--position-root-absolute);
  width: 20px;
  height: 20px;
  left: 0px;
  top: 0px;
  bottom: 0px;
  right: 0px;
}

.agree-text {
  position: var(--position-root-absolute);
  width: 463px;
  height: 72px;
  left: 40px;
  top: 0px;
  bottom: 0px;
  right: 0px;
  /* color */
  color: var(--color-text-secondary);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight400);
  font-size: var(--font-size14);
  line-height: var(--line-height24);
}

.agree-text strong {
  color: rgba(0, 0, 52, 1);
}

.btn-pay {
  position: var(--position-root-absolute);
  width: 515px;
  height: 56px;
  left: 0px;
  right: 0px;
  top: 100px;
  bottom: 40px;
  background: var(--color-text-primary);
  border-radius: 16px;
  cursor: pointer;
}

.btn-text3 {
  width: 161px;
  height: 20px;
  left:177px;
  right: 177px;
  top: 18px;
  bottom: 18px;
  text-decoration: none;
  /* color */
  color: rgba(255, 255, 255, 1);
  font-family: var(--font-primary-Poppins);
  font-style: var(--font-style-normal);
  font-weight: var(--font-weight600);
  font-size: var(--font-size16);
  line-height: var(--line-height20);
}







</style>
