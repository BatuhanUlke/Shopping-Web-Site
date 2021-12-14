# Shopping-Web-Site
<!DOCTYPE html>
<html>
<title>W3.CSS Template</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Montserrat">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
.w3-sidebar a {font-family: "Roboto", sans-serif}
body,h1,h2,h3,h4,h5,h6,.w3-wide {font-family: "Montserrat", sans-serif;}

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
body{
    margin:0px;
    padding: 0px;
    font-family: poppins;
    background-color: #ffffff;
}
*{
    box-sizing: border-box;
}
ul{
    list-style: none;
}
a{
    text-decoration: none;
}
nav{
    width:100%;
    box-shadow: 2px 2px 30px rgba(0,0,0,0.05);
    z-index: 100;
}
.social-call{
    height: 40px;
    border: 1px solid rgba(0,0,0,0.05);
    display: flex;
    justify-content: center;
    align-items: center;
}
.social a{
    margin: 0px 5px;
    color: rgba(0,0,0,0.7);
    font-size: 0.9rem;
}
.phone{
    color: rgba(0,0,0,0.7);
    margin-left: 30px;
    font-size: 0.9rem;
}
.social a:hover{
    color: #0b9d8a;
    transition: all ease 0.3s;
}
.navigation{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0px 45px;
}
.logo img{
    height: 30px;
}
.menu{
    display: flex;
}
.menu li{
    position: relative;
    margin: 20px;
    display: flex;
    text-transform: uppercase;
    font-weight: 500;
}
.menu li a{
    color: #555555;
}
.right-menu a{
    margin: 0px 10px;
    font-size: 1.2rem;
    color: rgba(0,0,0,0.7);
}
.menu a:hover,
.right-menu a:hover,
.search-cancel:hover,
.form-cancel:hover{
    color: #0b9d8a;
    transition: all ease 0.3s;
}
.sale-lable{
    width:38px;
    height: 17px;
    background-color: #f76b6a;
    color: #ffffff;
    font-weight: 400;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 0.7rem;
    text-transform: uppercase;
    position: absolute;
    top: -20px;
    right: -20px;
}
.sale-lable:after{
    content: '';
    width:0px;
    height: 0px;
    border-bottom: 5px solid transparent;
    border-left: 3px solid transparent;
    border-top: 7px solid #f76b6a;
    border-right: 5px solid transparent;
    position: absolute;
    left: 10%;
    top: 100%;
}
.fa-shopping-cart{
    position: relative;
}
.num-cart-product{
    position: absolute;
    top: -17px;
    right: -17px;
    width:25px;
    height: 25px;
    font-size: 0.8rem;
    border-radius: 50%;
    background-color: #0b9d8a;
    color: #ffffff;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 400;
}
.search-bar{
    width:100%;
    height: 300px;
    background-color: #ffffff;
    position: fixed;
    left: 0px;
    bottom: 0px;
    display: flex;
    justify-content: center;
    box-shadow: 2px -5px 30px rgba(0,0,0,0.1);
    z-index: 101;
    animation: search 0.3s;
}
.search-input{
    width:90%;
    border-bottom: 2px solid #555555;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100px;
    margin-top: 20px;
}
.search-bar input{
    width:100%;
    padding: 30px;
    border: none;
    outline: none;
    font-size: 2rem;
    margin: 20px;
    padding: 0px 20px;
}
.search-cancel{
    color: #272727;
    font-size: 2rem;
    padding-right: 40px;
}
.search-bar{
    display: none;
}
.search-bar-active{
    display: flex;
}
@keyframes search{
    0%{
        bottom: -300px;
    }
    100%{
        bottom: 0px;
    }
}
.form{
    width:100%;
    height: 100%;
    position: fixed;
    top: 0px;
    left: 0px;
    background-color: rgba(0,0,0,0.2);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    z-index: 102;
}
.login-form,
.sign-up-form{
    width:420px;
    padding: 20px 10px;
    background-color: #ffffff;
    box-shadow: 2px 2px 30px rgba(0,0,0,0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    border-radius: 5px;
    position: relative;
 
}
.login-form form,
.sign-up-form form{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 100%;
}
.login-form strong,
.sign-up-form strong{
    color: #272727;
    font-size: 2rem;
    margin: 2px 7px 7px 7px;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    font-weight: 500;
}
.login-form input,
.sign-up-form input{
    width:90%;
    height: 45px;
    margin: 6px 0px;
    padding: 0px 10px;
    border: 1px solid rgba(0,0,0,0.1);
    outline: none;
    border-radius: 7px;
}
.login-form input::placeholder,
.sign-up-form input::placeholder{
    color: rgba(0,0,0,0.5);
}
.login-form input[type="submit"],
.sign-up-form input[type="submit"]{
    background-color: #0b9d8a;
    color: #ffffff;
    border: none;
    outline: none;
    text-transform: uppercase;
    margin-top: 10px;
    border-radius: 3px;
    box-shadow: 2px 2px 30px rgba(0,0,0,0.1);
}
.form-btns{
    width: 90%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 10px;
}
.form-btns a{
    color: #4d4d4d;
    font-size: 0.9rem;
}
.sign-up-btn{
    border-bottom: 1px solid #868686;
    line-height: 16px;
}
.form-cancel{
    position: absolute;
    right: 20px;
    top: 10px;
    color: #868686;
}
.login-form,
.sign-up-form,
.form{
    display: none;
}
.login-active,
.login-active .login-form{
    display: flex;
    animation: fade 0.3s;
}
 
.sign-up-active,
.sign-up-active .sign-up-form{
    display: flex;
    animation: fade 0.3s;
}
@keyframes fade{
    0%{
        opacity: 0;
    }
    100%{
        opacity: 1;
    }
}
</style>
<body class="w3-content" style="max-width:1200px">

<!-- Sidebar/menu -->
<nav class="w3-sidebar w3-bar-block w3-white w3-collapse w3-top" style="z-index:3;width:250px" id="mySidebar">
  <div class="w3-container w3-display-container w3-padding-16">
    <i onclick="w3_close()" class="fa fa-remove w3-hide-large w3-button w3-display-topright"></i>
    <h3 class="w3-wide"><b>JUAN</b></h3>
  </div>
  <div class="w3-padding-64 w3-large w3-text-grey" style="font-weight:bold">
    <a href="shirts.html" class="w3-bar-item w3-button">Shirts</a>
   
    <a href="dresses.html" class="w3-bar-item w3-button">Dresses</a>
    <a onclick="myAccFunc()" href="javascript:void(0)" class="w3-button w3-block w3-white w3-left-align" id="myBtn">
      Jeans <i class="fa fa-caret-down"></i>
    </a>
    
    <a href="jacket.html" class="w3-bar-item w3-button">Jackets</a>
    <a href="cometics.html" class="w3-bar-item w3-button">Cosmetics</a>
    <a href="blazer.html" class="w3-bar-item w3-button">Blazers</a>
    <a href="shoes.html" class="w3-bar-item w3-button">Shoes</a>
  </div>
  <a href="#footer" class="w3-bar-item w3-button w3-padding">Contact</a> 
  <a href="javascript:void(0)" class="w3-bar-item w3-button w3-padding" onclick="document.getElementById('newsletter').style.display='block'">Newsletter</a> 
  <a href="#footer"  class="w3-bar-item w3-button w3-padding">Subscribe</a>
</nav>

<!-- Top menu on small screens -->
<header class="w3-bar w3-top w3-hide-large w3-black w3-xlarge">
  <div class="w3-bar-item w3-padding-24 w3-wide">JUAN</div>
  <a href="javascript:void(0)" class="w3-bar-item w3-button w3-padding-24 w3-right" onclick="w3_open()"><i class="fa fa-bars"></i></a>
</header>

<!-- Overlay effect when opening sidebar on small screens -->
<div class="w3-overlay w3-hide-large" onclick="w3_close()" style="cursor:pointer" title="close side menu" id="myOverlay"></div>

<!-- !PAGE CONTENT! -->
<div class="w3-main" style="margin-left:250px">

  <!-- Push down content on small screens -->
  <div class="w3-hide-large" style="margin-top:83px"></div>
  
  <!-- Top header -->
  <header class="w3-container w3-xlarge">
    <p class="w3-left">Jeans</p>
    <p class="w3-right">
      
      <a href="javascript:void(0);" class="search">
        <i class="fas fa-search"></i>
        <a href="javascript:void(0);" class="user">
          <i class="far fa-user"></i>
          <a href="#">
            <i class="fas fa-shopping-cart">
                <span class="num-cart-product">0</span>
            </i>
        </a>
      </a>
    </a>
    </p>
  </header>
  <div class="search-bar">
    
    <!--search-input------->
    <div class="search-input">
    <input type="text" placeholder="Search For Product" name="search" />
    <!--cancel-btn--->
    <a href="javascript:void(0);" class="search-cancel">
        <i class="fas fa-times"></i>
    </a>

</div>
</div>
<!---login-and-sign-up--------------------------------->
<div class="form">
  <!--login---------->
  <div class="login-form">
      <!--cancel-btn---------------->
      <a href="javascript:void(0);" class="form-cancel">
          <i class="fas fa-times"></i>
      </a>
      <strong>Log In</strong>
      <!--inputs-->
      <form>
          <input type="email" name="email" placeholder="Example@gmail.com" required/>
          <input type="password" name="password" placeholder="Password" required/>
          <input type="submit" value="Log In"/>
      </form>
      <!--forget-and-sign-up-btn-->
      <div class="form-btns">
          <a href="#" class="forget">Forget Your Password?</a>
          <a href="javascript:void(0);" class="sign-up-btn">Create Account</a>
      </div>
  </div>
      <!--Sign-up---------->
      <div class="sign-up-form">
          <!--cancel-btn---------------->
      <a href="javascript:void(0);" class="form-cancel">
          <i class="fas fa-times"></i>
      </a>
          <strong>Sign Up</strong>
          <!--inputs-->
          <form>
              <input type="text" name="fullname" placeholder="Full Name" required/>
              <input type="email" name="email" placeholder="Example@gmail.com" required/>
              <input type="password" name="password" placeholder="Password" required/>
              <input type="submit" value="Sign Up"/>
          </form>
          <!--forget-and-sign-up-btn-->
          <div class="form-btns">
              <a href="javascript:void(0);" class="already-account">
                  Already Have Account?</a>

          </div>
      </div>
</div>



  <!-- Image header -->
  <div class="w3-display-container w3-container">
    <img src="img/new.jfif" alt="Jeans" style="width:100%">
    <div class="w3-display-topleft w3-text-white" style="padding:24px 48px">
      <h1 class="w3-jumbo w3-hide-small">New arrivals</h1>
      <h1 class="w3-hide-large w3-hide-medium">New arrivals</h1>
      <h1 class="w3-hide-small">COLLECTION 2021</h1>
      <p><a href="#jeans" class="w3-button w3-black w3-padding-large w3-large">SHOP NOW</a></p>
    </div>
  </div>

  <div class="w3-container w3-text-grey" id="jeans">
    <p>8 items</p>
  </div>
  <!-- Product grid by jeans -->

  <!-- Product grid by jeans -->
  <div class="w3-row w3-grayscale">
    <div class="w3-col l3 s6">
      <div class="w3-container">
        <img src="img/Blue Knee Rip Baggy Pants.jfif" style="width:100%">
        <span class="w3-tag w3-display-topleft">New</span>
          <div class="w3-display-middle w3-display-hover">
            <button class="w3-button w3-black">Buy now <i class="fa fa-shopping-cart"></i></button>
          </div>
        <p>Blue Knee Rip Baggy Jeans<br><b>$20.99</b></p>
      </div>
      <div class="w3-container">
        <img src="img/flared higher jean.jfif" style="width:100%">
        
        <p>Flared Higher Jean<br><b>$15.99</b></p>
      </div>
    </div>

    <div class="w3-col l3 s6">
      <div class="w3-container">
        <div class="w3-display-container">
          <img src="img/mom jean.jfif" style="width:100%">
          <span class="w3-tag w3-display-topleft">New</span>
          <div class="w3-display-middle w3-display-hover">
            <button class="w3-button w3-black">Buy now <i class="fa fa-shopping-cart"></i></button>
          </div>
        </div>
        <p>Mom Jean<br><b>$19.99</b></p>
      </div>
      <div class="w3-container">
        <img src="img/old school jeans.jfif" style="width:100%">
        <p>Old School Jean<br><b>$10.50</b></p>
      </div>
    </div>

    <div class="w3-col l3 s6">
      <div class="w3-container">
        <img src="img/relaxed jeans.jfif" style="width:100%">
        <p>Relaxed Jean<br><b>$17.50</b></p>
      </div>
      <div class="w3-container">
        <div class="w3-display-container">
          <img src="img/skinny jeans.jfif" style="width:100%">
          <span class="w3-tag w3-display-topleft">Sale</span>
          <div class="w3-display-middle w3-display-hover">
            <button class="w3-button w3-black">Buy now <i class="fa fa-shopping-cart"></i></button>
          </div>
        </div>
        <p> Skinny Jeans<br><b class="w3-text-red">$14.99</b></p>
      </div>
    </div>

    <div class="w3-col l3 s6">
      <div class="w3-container">
        <img src="img/skinny jeans.jfif" style="width:100%">
        <p> Skinny Jeans<br><b>$14.99</b></p>
      </div>
      <div class="w3-container">
        <img src="img/washed jean.jfif" style="width:100%">
        <p>Washed Jean<br><b>$24.99</b></p>
      </div>
    </div>
  </div>

  <!-- Subscribe section -->
  <div class="w3-container w3-black w3-padding-32">
    <h1>Subscribe</h1>
    <p>To get special offers and VIP treatment:</p>
    <p><input class="w3-input w3-border" type="text" placeholder="Enter e-mail" style="width:100%"></p>
    <button type="button" class="w3-button w3-red w3-margin-bottom">Subscribe</button>
  </div>
  
  <!-- Footer -->
  <footer class="w3-padding-64 w3-light-grey w3-small w3-center" id="footer">
    <div class="w3-row-padding">
      <div class="w3-col s4">
        <h4>Contact</h4>
        <p>Questions? Go ahead.</p>
        <form action="/action_page.php" target="_blank">
          <p><input class="w3-input w3-border" type="text" placeholder="Name" name="Name" required></p>
          <p><input class="w3-input w3-border" type="text" placeholder="Email" name="Email" required></p>
          <p><input class="w3-input w3-border" type="text" placeholder="Subject" name="Subject" required></p>
          <p><input class="w3-input w3-border" type="text" placeholder="Message" name="Message" required></p>
          <button type="submit" class="w3-button w3-block w3-black">Send</button>
        </form>
      </div>

      <div class="w3-col s4">
        <h4>About</h4>
        <p><a href="#">About us</a></p>
        <p><a href="#">We're hiring</a></p>
        <p><a href="#">Support</a></p>
        <p><a href="#">Find store</a></p>
        <p><a href="#">Shipment</a></p>
        <p><a href="#">Payment</a></p>
        <p><a href="#">Gift card</a></p>
        <p><a href="#">Return</a></p>
        <p><a href="#">Help</a></p>
      </div>

      <div class="w3-col s4 w3-justify">
        <h4>Store</h4>
        <p><i class="fa fa-fw fa-map-marker"></i> Company Name</p>
        <p><i class="fa fa-fw fa-phone"></i> 0044123123</p>
        <p><i class="fa fa-fw fa-envelope"></i> ex@mail.com</p>
        <h4>We accept</h4>
        <p><i class="fa fa-fw fa-cc-amex"></i> Amex</p>
        <p><i class="fa fa-fw fa-credit-card"></i> Credit Card</p>
        <br>
        <i class="fa fa-facebook-official w3-hover-opacity w3-large"></i>
        <i class="fa fa-instagram w3-hover-opacity w3-large"></i>
        <i class="fa fa-snapchat w3-hover-opacity w3-large"></i>
        <i class="fa fa-pinterest-p w3-hover-opacity w3-large"></i>
        <i class="fa fa-twitter w3-hover-opacity w3-large"></i>
        <i class="fa fa-linkedin w3-hover-opacity w3-large"></i>
      </div>
    </div>
  </footer>

  <div class="w3-black w3-center w3-padding-24">Powered by Batuhan Ulke</div>
  <!-- End page content -->
</div>

<!-- Newsletter Modal -->
<div id="newsletter" class="w3-modal">
  <div class="w3-modal-content w3-animate-zoom" style="padding:32px">
    <div class="w3-container w3-white w3-center">
      <i onclick="document.getElementById('newsletter').style.display='none'" class="fa fa-remove w3-right w3-button w3-transparent w3-xxlarge"></i>
      <h2 class="w3-wide">NEWSLETTER</h2>
      <p>Join our mailing list to receive updates on new arrivals and special offers.</p>
      <p><input class="w3-input w3-border" type="text" placeholder="Enter e-mail"></p>
      <button type="button" class="w3-button w3-padding-large w3-red w3-margin-bottom" onclick="document.getElementById('newsletter').style.display='none'">Subscribe</button>
    </div>
  </div>
</div>
<!--using JQuery--------------->
<script
  src="https://code.jquery.com/jquery-3.5.1.js" integrity="sha256-QWo7LDvxbWT2tbbQ97B53yJnYU3WhH/C8ycbRAkjPDc=" crossorigin="anonymous"></script>

 <!--using FontAwesome--------------->
 <script crossorigin="anonymous" src="https://kit.fontawesome.com/c8e4d183c2.js"></script>
<script>
// Accordion 
function myAccFunc() {
  var x = document.getElementById("demoAcc");
  if (x.className.indexOf("w3-show") == -1) {
    x.className += " w3-show";
  } else {
    x.className = x.className.replace(" w3-show", "");
  }
}

// Click on the "Jeans" link on page load to open the accordion for demo purposes
document.getElementById("myBtn").click();


// Open and close sidebar
function w3_open() {
  document.getElementById("mySidebar").style.display = "block";
  document.getElementById("myOverlay").style.display = "block";
}
 
function w3_close() {
  document.getElementById("mySidebar").style.display = "none";
  document.getElementById("myOverlay").style.display = "none";
}
/*-----For Search Bar-----------------------------*/
$(document).on('click','.search',function(){
        $('.search-bar').addClass('search-bar-active')
    });
 
    $(document).on('click','.search-cancel',function(){
        $('.search-bar').removeClass('search-bar-active')
    });
        $(document).on('click','.user,.already-account',function(){
        $('.form').addClass('login-active').removeClass('sign-up-active')
    });
 
    $(document).on('click','.sign-up-btn',function(){
        $('.form').addClass('sign-up-active').removeClass('login-active')
    });
 
    $(document).on('click','.form-cancel',function(){
        $('.form').removeClass('login-active').removeClass('sign-up-active')
    });
 
</script>

</body>
</html>
