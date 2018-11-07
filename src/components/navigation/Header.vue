<template>
    <div class="top">
      <nav class="navbar navbar-default header-view" >
        <div class="container">
          <div class="navbar-header">
            <div class="login-btn small-screen">
                <a class="dropdown-toggle header-link" @click="showLogin()" role="button" style="color:#fff">Log in/Sign up</a>
            </div>
            <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
              <span class="sr-only">Toggle navigation</span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
            </button>
            <div class="logo">
                <router-link to="/">
                <img src="../../assets/img/logo_top.png" alt=""> 
                </router-link>
           </div>
          </div>
          <div id="navbar" class="navbar-collapse collapse">
            <ul class="nav navbar-nav navbar-right">
              <li class="dropdown">
                <a class="dropdown-toggle header-link"  role="button">Find a Provider</a>

              </li>
              <li class="dropdown">
                <a class="dropdown-toggle header-link"  role="button"  >Find a Facility</a>
              </li>
              <li class="dropdown login-btn hide-for-small-screen">
                <a class="dropdown-toggle header-link" @click="showLogin()" role="button" style="color:#fff">Log in/Sign up</a>
              </li>
              <li class="hide-for-small-screen">
                <router-link to="" class="header-link"> 
                  <i class="fas fa-search"></i>
                </router-link>
                
              </li>
            </ul>
          </div><!--/.nav-collapse -->
        </div><!--/.container-fluid -->
      </nav>
      <div class="login-srch-form" v-show="login">
							<div class="login-srch-form-wpr">
								<h2>Log In</h2>
								<form>
									<div class="use-links">
										<button class="cta-green"><img src="../../assets/img/google-icon.png" alt="">Use Google Contact</button>
										<button class="cta-green"><img src="../../assets/img/fb-icon.png" alt="">Continue with Facebook</button>
									</div>
									<div class="or"><span>Or</span></div>
								
									<div class="login-srch-forn-inr">
										<label>Email</label>
										<input type="text" placeholder="abc@gmail.com">
									</div>
									<div class="login-srch-forn-inr">
										<label>Password</label>
										<input type="password" placeholder="">
									</div>
									<button class="cta-green">Log In</button>
								</form>
								<div class="forgot-pwd">
									<a href="#">Forgot Password?</a>
								</div>
								<div class="signup">
									<span>Don't have an account? <a href="#">Sign Up</a></span>
								</div>
							</div>
		</div>
      <div class="top-content">
            <div class="">
                <h1>
                  A health directory For you and your Family
                </h1>
              <div class="search-content">
                 <div class="row"> 
                  <div class="col-md-6 col">
                    <div class="input-group">
                      <span class="input-group-addon">Search</span>
                      <input id="emailn" type="text" class="form-control" name="email" placeholder="Facilities, Providers, Services">
                    </div>
                  </div>
                  <div class="col-md-4 col">
                    <div class="input-group">
                      <span class="input-group-addon">Near</span>
                      <input id="email" type="text" class="form-control" name="email" placeholder="City, State">
                    </div>
                  </div>
                  <div class="col-md-2 col">
                    <button class="btn full-width search-btn">
                      Search
                    </button>
                  </div>
                </div>
              </div>

            </div>
      </div>
    </div>
</template>
<script>

export default {
  data () {
    return {
    login:false
    }
  },
  methods:{
      showLogin(){
          if(this.login){
               this.login = false;
          }else{
               this.login = true;
          }
         
      }
    
  }
}

</script>
<style scoped>

.top{
  background-image:url('../../assets/img/bg_img.png');
  background-position: 36% 11px;
    background-repeat: no-repeat;
    height: 639px;
    background-size: cover;
}

.header-view{
  padding: 10px 0;
  background: #fff;
  border: 0;
  border-bottom: 1px solid #9a929240;
}

 .header-link{
    color: #000;
    font-weight: 500;
    font-size: 15px;
  }

.top-content{
    text-align: center;
    color: #fff;
    width: 72%;
    margin: 150px auto;
}

.top-content h1{
  margin-bottom: 60px;
 font-size: 45px;
 font-weight: bold;
}

.top-content .col{
  padding: 0;
  padding:0 5px
}

.input-group-addon{
  color: #615b5b;
  background: #fff;
  font-weight: bold;
  font-size: 17px;
}

.form-control{
    padding: 24px 12px;
    font-size: 17px;
    font-weight: bold;
}
.top-content .input-group-addon, .top-content .form-control {
  border:0 !important;
  box-shadow: none !important;
}

.full-width{
  width: 100%;
}
.search-btn{
  background:#FF3D00;
  padding: 11px 0;
  font-size: 17px;
   font-weight: bold;
}

.col button:focus,.col button:hover {
    color:#fff;
    outline: 0;

}

.login-btn a{
    background: #02B175;
    border-radius: 3px;
    margin: 4px 0 0px;
    padding: 10px;
    font-weight: bold;
}

.login-btn a:hover{
    background: #089061 !important;
    color:#fff !important;
}

.form-control:focus {
    outline: 0;
    -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102,175,233,.6);
    box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(224, 224, 224, 0.6);
}

.search-content{
    padding: 0px 105px;
}

.navbar-default .navbar-nav>li>a {
    color: #1b1a1a;
    font-weight: bold;
}

.logo{
    margin: 11px 0;
    max-width: 150px;
}

.logo img{
    width: 100%;
}

.login-srch-form {
    position: absolute;
    top:71px;
    background: #fff;
    box-shadow: rgba(0,0,0,.2) 0 0 15px;
   right: 144px;
    min-width: 330px;
    /* visibility: hidden; */
    max-height: calc(100vh - 80px);
    overflow-y: auto;
    width: 350px;
    z-index: 566;
}

.login-srch-form-wpr {
    width: 100%;
    float: left;
    padding: 30px;
}

.login-srch-form-wpr h2{
    text-align: left;
}

.login-srch-form h2 {
    font-size: 35px;
    color: #02b176;
    font-weight: 700;
}

.login-srch-form .use-links {
    width: 100%;
    float: left;
}

.login-srch-form .use-links button {
    margin: 20px 0 0;
    background-color: #fff;
    color: #000;
    box-shadow: rgba(0,0,0,.2) 0 0 5px;
    position: relative;
}
.login-srch-form button {
    background-color: #ff3f00;
    width: 100%;
}
.cta-green {
    display: inline-block;
    font-size: 14px;
    text-align: center;
    padding: 13px 25px;
    line-height: 1;
    transition: .2s;
    background-color: #02b176;
    color: #fff;
    border-radius: 5px;
}
button {
    cursor: pointer;
}

.login-srch-form .use-links button img {
    max-width: 14px;
    position: absolute;
    left: 15px;
    top: 50%;
    transform: translateY(-50%);
}

.login-srch-form .use-links button {
    margin: 20px 0 0;
    background-color: #fff;
    color: #000;
    box-shadow: rgba(0,0,0,.2) 0 0 5px;
    position: relative;
}

.login-srch-form .or {
    width: 100%;
    float: left;
    text-align: center;
    position: relative;
    margin: 20px 0;
}

.login-srch-forn-inr {
    width: 100%;
    float: left;
    margin: 0 0 20px;
}
.login-srch-forn-inr label {
    display: inline-block;
    width: 100%;
    font-size: 16px;
    margin: 0 0 10px;
    color: #02b176;
        text-align: left;
}

.login-srch-form input {
    width: 100%;
    padding: 10px;
    border: 1px solid #ddd;
    line-height: 1;
    display: inline-block;
    font-size: 14px;
}

.login-srch-forn-inr {
    width: 100%;
    float: left;
    margin: 0 0 20px;
}
.login-srch-form button {
    background-color: #ff3f00;
    width: 100%;
}
.login-srch-forn-inr label {
    display: inline-block;
    width: 100%;
    font-size: 16px;
    margin: 0 0 10px;
    color: #02b176;
}

.forgot-pwd {
    width: 100%;
    float: left;
    margin: 20px 0 15px;
    text-align: center;
}
.login-srch-form .forgot-pwd a {
    display: inline-block;
    font-size: 14px;
    color: #9e9f9e;
}
.login-srch-form .signup {
    width: 100%;
    float: left;
    text-align: center;
}
.login-srch-form .signup span {
    display: inline-block;
    font-size: 14px;
    color: #9e9f9e;
}

.small-screen{
    display: none;
}

@media (max-width: 767px)
{

.logo{
    margin: 11px 13px;
    max-width: 154px;
     width: 112px;
}
.navbar-default .navbar-toggle {
    border: none;
}

.navbar-default .navbar-toggle .icon-bar {
    background-color: #1d1c1c;
}

.navbar-default .navbar-toggle:focus, .navbar-default .navbar-toggle:hover {
    background-color: #ddd;
    background: transparent;
}

.small-screen{
    display: block;
    position: absolute;
    right: 64px;
    top: 23px;
}

.hide-for-small-screen{
    display:none;
}

.navbar-default .navbar-nav>li>a{
    color: #ffffff;
    text-align: left;
}

.header-view{
    padding: 10px 0 0;
    border: 0;
}

.navbar-default .navbar-collapse, .navbar-default .navbar-form {
    background: #021933;
}

.nav>li {
    border-bottom: 1px solid #d3d3d3;
    margin: 0;
}

.nav>li:nth-last-child(3){
    border:none;
}

.top-content{
    width: 100%;
    margin: 135px auto;
}

.top-content h1{
    margin-bottom: 55px;
    font-size: 36px;
}

.search-content{
    padding: 0px 25px;
}

.top-content .col {
    margin-bottom: 21px;
}

.top {
    background-position: 49% 11px;
}

.login-srch-form{
    top: 58px;
    right: 10px;
    min-width: 330px;
    width: 324px;
}

}
</style>

