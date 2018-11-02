<template>
    <div class="top">
      <nav class="navbar navbar-default header-view" >
        <div class="container">
          <div class="navbar-header">
            <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
              <span class="sr-only">Toggle navigation</span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
            </button>
            <router-link to="/">
            <img src="../../assets/img/logo.png" alt="" class="logo"> 
            <span style="font-size: 22px;font-weight: bold;">| Navi Health</span>
            </router-link>
          </div>
          <div id="navbar" class="navbar-collapse collapse">
            <ul class="nav navbar-nav navbar-right">
              <li class="dropdown">
                <a class="dropdown-toggle header-link"  role="button">Find a Provider</a>

              </li>
              <li class="dropdown">
                <a class="dropdown-toggle header-link"  role="button"  >Find a Facility</a>
              </li>
              <li class="dropdown login-btn">
                <a class="dropdown-toggle header-link"  role="button">Log in/Sign up</a>
              </li>
              <li>
                <router-link to="" class="header-link"> 
                  <i class="fas fa-search"></i>
                </router-link>
                
              </li>
            </ul>
          </div><!--/.nav-collapse -->
        </div><!--/.container-fluid -->
      </nav>
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
                      <input id="email" type="text" class="form-control" name="email" placeholder="Facilities, Providers, Services">
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

</script>
<style scoped>

.top{
  background-image:url('../../assets/img/bg_img.png');
  background-position: 45% -10px;
  background-repeat: no-repeat;
  height: 500px;
  /* background-size: cover; */
}

.header-view{
  padding: 10px 0;
  background: transparent;
  border: 0;
  border-bottom: 1px solid #9a929240;
}

 .header-link{
    color: #ffffff !important;
    font-weight: bold;
  }

.top-content{
    text-align: center;
    color: #fff;
    width: 70%;
    margin: 150px auto;
}

.top-content h1{
  margin-bottom: 60px;
 font-size: 45px;
}

.top-content .col{
  padding: 0;
  padding:0 5px
}

.input-group-addon{
  color: #615b5b;
  background: #fff;
  font-weight: bold;
}

.form-control{
      padding: 22px 12px;
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
}

.col button:focus,.col button:hover {
    color:#fff;
    outline: 0;

}

.login-btn a{
    background: #02B175;
    padding-top: 10px;
    padding-bottom: 10px;
    border-radius: 3px;
}

.login-btn a:hover{
    background: #02B175 !important;
}

.form-control:focus {
    outline: 0;
    -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102,175,233,.6);
    box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(224, 224, 224, 0.6);
}

.search-content{
    padding: 0px 105px;
}

</style>

