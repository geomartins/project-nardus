
<template>
  <!--header start-->
  <header id="masthead" class="header ttm-header-style-01">
    <!-- ttm-header-wrap -->
    <div class="ttm-header-wrap">
      <!-- ttm-stickable-header-w -->
      <div id="ttm-stickable-header-w" class="ttm-stickable-header-w clearfix">
        <!-- ttm-topbar-wrapper -->
        <div class="ttm-topbar-wrapper clearfix">
          <div class="container">
            <div class="row">
              <div class="col-lg-12">
                <div class="ttm-topbar-content">
                  <ul class="top-contact text-left">
                    <li>Pure Aroma From Nature</li>
                  </ul>
                  <div class="topbar-right text-right">
                    <ul class="top-contact">
                      <li>Office Hour : 08:00am - 5:00pm</li>
                    </ul>
                    <div class="ttm-social-links-wrapper list-inline">
                      <ul class="social-icons">
                        <li>
                          <a href="#"><i class="fa fa-facebook"></i></a>
                        </li>
                        <li>
                          <a href="https://twitter.com/nardusltd"><i class="fa fa-twitter"></i></a>
                        </li>
                        <li>
                          <a href="https://www.instagram.com/nardusltd/"><i class="fa fa-instagram"></i></a>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- ttm-topbar-wrapper end -->
        <div class="ttm-widget_header">
          <div class="container">
            <div class="row">
              <div class="col-lg-12">
                <div class="d-flex flex-row align-items-center">
                  <!-- site-branding -->
                  <div class="site-branding mr-auto">
                       <router-link to="/" tag="a" class="home-link" title="Nardus"
                      rel="home" > 
                   
                      <img
                        src="img/logo.jpg"
                        id="logo-img"
                        class="img-center"
                        alt="logo"
                      />
                    </router-link>
                  </div>
                  <!-- site-branding end -->
                  <!-- widget-info -->
                  <div
                    class="widget_info d-flex flex-row align-items-center justify-content-end"
                  >
                    <div class="widget_icon"><i class="flaticon-call"></i></div>
                    <div class="widget_content">
                      <h5 class="widget_title">(234) 906-282-2260</h5>
                      <p class="widget_desc">Make A Call</p>
                    </div>
                  </div>
                  <!-- widget-info end -->
                  <!-- widget-info -->
                  <div
                    class="widget_info d-flex flex-row align-items-center justify-content-end"
                  >
                    <div class="widget_icon">
                      <i class="flaticon-email"></i>
                    </div>
                    <div class="widget_content">
                      <h5 class="widget_title">info@nardus.ng</h5>
                      <p class="widget_desc">Send Us a Mail </p>
                    </div>
                  </div>
                  <!-- widget-info end -->
                  <!-- widget-info -->
                  <div
                    class="widget_info d-flex flex-row align-items-center justify-content-end"
                  >
                    <div class="widget_icon">
                      <i class="flaticon-worldwide"></i>
                    </div>
                    <div class="widget_content">
                      <h5 class="widget_title">Osborne Foreshore, Ikoyi, Lagos, Nigeria</h5>
                      <p class="widget_desc">18 Udi street, Wema Terrace</p>
                    </div>
                  </div>
                  <!-- widget-info end -->
                </div>
              </div>
            </div>
          </div>
        </div>
        <div id="site-header-menu" class="site-header-menu">
          <div class="site-header-menu-inner ttm-stickable-header">
            <div class="container">
              <!--site-navigation -->
              <div id="site-navigation" class="site-navigation">
                <div class="ttm-custombutton">
                     <router-link to="/contact" tag="a" class="ttm-btn ttm-btn-size-md ttm-btn-bgcolor-skincolor"> Request for quote </router-link>
                 
                </div>
                <!-- header-icons -->
                <div class="ttm-header-icons ">
                  <span class="ttm-header-icon ttm-header-cart-link">
                    <a href="#"
                      ><i class="fa fa-shopping-cart"></i>
                      <span class="number-cart">0</span>
                    </a>
                  </span>
         
                </div>
                <!-- header-icons end -->
                <div class="ttm-menu-toggle">
                  <input type="checkbox" :class="{ active: menuStatus }" id="menu-toggle-form" />
                  <label for="menu-toggle-form" class="ttm-menu-toggle-block" @click="activate()">
                    <span class="toggle-block toggle-blocks-1"></span>
                    <span class="toggle-block toggle-blocks-2"></span>
                    <span class="toggle-block toggle-blocks-3"></span>
                  </label>
                </div>
                <nav id="menu" class="menu" :class="{ active: menuStatus }" >
                  <ul class="dropdown">
                   
                        <router-link to="/" tag="li" exact-active-class="active" exact> <a> Home </a> </router-link>
                  
                        <router-link to="/about" tag="li" exact-active-class="active" exact > <a> About Us </a></router-link>
                    
                  
                        <router-link to="/services"  tag="li" exact-active-class="active" exact ><a> Services </a> </router-link>
                    
                   
                      <router-link to="/faq"  tag="li" exact-active-class="active" exact> <a> Faq </a></router-link>
                     
                    
                      <router-link to="/shop"  tag="li" exact-active-class="active" exact><a> Shop </a> </router-link>
                     
                      
                   
                    
                      <router-link to="/contact"  tag="li" exact-active-class="active" exact > <a> Contact Us </a></router-link>
                      
                    
                  </ul>
                </nav>
              </div>
              <!-- site-navigation end-->
            </div>
          </div>
        </div>
      </div>
      <!-- ttm-stickable-header-w end-->
    </div>
    <!--ttm-header-wrap end -->
  </header>
  <!--header end-->
</template>

<script>
export default {
  name: "Header",
  props: {},
  data(){
    return {
      menuStatus: false
    }
  },
  methods: {
    activate: function(){
      this.menuStatus = !this.menuStatus;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style></style>
