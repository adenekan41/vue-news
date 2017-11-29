<template>
  <div id="app">
    <div class="h-t">
      <Navbar></Navbar>
      <h1 class="text-center tet"><i class="text-danger">News</i><b>Works</b>.io</h1><br>
        <div class="container-fluid" style="padding-bottom: 10px;">
          <div class="row">
          <div class="col-md-3">
          </div>
          <div class="col-md-6 ">
            <form>
              <div class="input-group">
                <input type="text" class="form-control" placeholder="Search" style="border: none !important; ">
                <div class="input-group-btn">
                  <button class="btn btn-default" type="submit" style="border-radius: 1px; background-color:#dab114;color: white; border: 1px solid rgb(218, 177, 20);">
                    Search News
                  </button>
                </div>
              </div>
          </form>
          </div>
        
          
          <div class="col-md-3">
          </div>
        </div><br>
        </div>
      <center>
        <a class="btn btn-md btn-warning" href="#" style="background-color:transparent; border-radius: 50px; color: #fff; padding: 6px 35px; border: 2px solid #ffd600;" role="button">Learn more</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        <a class="btn btn-md btn-warning" href="#" style="background-color:rgba(255, 214, 0, 0.4); border-radius: 50px; border:none; padding:6px 35px; border: 2px solid #ffd600; color: white;" role="button">Get Api Key</a>
      </center>
    </div>
    <div class="container">
      <header>
      <nav class="navbar navbar-default navbar-static-top">
        <div class="container-fluid">
          <div class="navbar-header">
            <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#myNavbar">
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>                        
            </button>
            <a class="navbar-brand" href="#"><i class="text-danger">News</i>Works</a>
          </div>
          <div class="collapse navbar-collapse" id="myNavbar">
            <ul class="nav navbar-nav">
             
              <li><a href="#">News Apis</a></li>
              <li><a href="#">CNN</a></li>
              <li><a href="#">Aljazera</a></li>
              <li><a href="#">Bilber News</a></li>
              <li><a href="#">Tvc News</a></li>
              <li><a href="#">Rio News</a></li>
              <li><a href="#">Goal News</a></li>
              <li><a href="#">Bcc Sport</a></li>
              <li><a href="#">Night News</a></li>
              <li><a href="#">Titu timuna</a></li>
            </ul>
          </div>
        </div>
      </nav>
  
    </header>
    </div>
    <Sliders></Sliders><br><br>
    <div class="container-fluid bg2">
      <div class="row">
        <div class="col-md-3">
          <LeftBar></LeftBar>
        </div>
        <div class="col-md-6">
          <SourceSelection v-on:sourceChanged="sourceChanged"></SourceSelection>
          <NewsList v-bind:source="source"></NewsList>
        </div>
        <div class="col-md-3">
          <RightBar></RightBar>
        </div>

      </div>
    </div>

<footer>
    <div class="footer" id="footer">
        <div class="container">
            <div class="row">
                <div class="col-lg-2  col-md-2 col-sm-4 col-xs-6">
                    <h3> Latest News </h3>
                    <ul>
                        <li> <a href="#"> Bussiness </a> </li>
                        <li> <a href="#"> Football </a> </li>
                        <li> <a href="#"> Finance </a> </li>
                        <li> <a href="#"> Security </a> </li>
                    </ul>
                </div>
                <div class="col-lg-2  col-md-2 col-sm-4 col-xs-6">
                    <h3> Top News </h3>
                    <ul>
                        <li> <a href="#"> Marketing </a> </li>
                        <li> <a href="#"> Space Punch </a> </li>
                        <li> <a href="#"> Histogrammy </a> </li>
                        <li> <a href="#"> Workars </a> </li>
                    </ul>
                </div>
                <div class="col-lg-2  col-md-2 col-sm-4 col-xs-6">
                    <h3> Programmes </h3>
                    <ul>
                        <li> <a href="#"> Lorem Ipsum </a> </li>
                        <li> <a href="#"> Flakeys </a> </li>
                        <li> <a href="#"> Intreomary </a> </li>
                        <li> <a href="#"> Maps </a> </li>
                    </ul>
                </div>
                <div class="col-lg-2  col-md-2 col-sm-4 col-xs-6">
                    <h3> Old News </h3>
                    <ul>
                        <li> <a href="#"> 1885 </a> </li>
                        <li> <a href="#"> 1990 </a> </li>
                        <li> <a href="#"> 1991 </a> </li>
                        <li> <a href="#"> 2000 </a> </li>
                    </ul>
                </div>
                <div class="col-lg-3  col-md-3 col-sm-6 col-xs-12 ">
                    <h3> Lorem Ipsum </h3>
                    <ul>
                        <li>
                            <input type="text" name="" class="form-control" placeholder="Your Email">
                            <button class="btn btn-warning btn-group-justified">Get Apis</button>
                        </li>
                    </ul>
                    <ul class="social">
                        <li> <a href="#"> <i class=" fa fa-facebook">   </i> </a> </li>
                        <li> <a href="#"> <i class="fa fa-twitter">   </i> </a> </li>
                        <li> <a href="#"> <i class="fa fa-google-plus">   </i> </a> </li>
                        <li> <a href="#"> <i class="fa fa-pinterest">   </i> </a> </li>
                        <li> <a href="#"> <i class="fa fa-youtube">   </i> </a> </li>
                    </ul>
                </div>
            </div>
            <!--/.row--> 
        </div>
        <!--/.container--> 
    </div>
    <!--/.footer-->
    
    <div class="footer-bottom">
        <div class="container">
            <p class="pull-left"> Copyright © <i class="text-danger">News</i>Works.io 2017. All right reserved. </p>
            <div class="pull-right">
                <ul class="nav nav-pills payments">
                    <li><i class="fa fa-cc-visa"></i></li>
                    <li><i class="fa fa-cc-mastercard"></i></li>
                    <li><i class="fa fa-cc-amex"></i></li>
                    <li><i class="fa fa-cc-paypal"></i></li>
                </ul> 
            </div>
        </div>
    </div>
    <!--/.footer-bottom--> 
</footer>
  </div>
</template>

<script>
import SourceSelection from './components/SourceSelection'
import NewsList from './components/NewsList'
import Navbar from './components/Navbar'
import LeftBar from './components/LeftBar'
import RightBar from './components/RightBar'
import Sliders from './components/Sliders'

export default {
  name: 'app',
  components: {
    SourceSelection,
    NewsList,
    Navbar,
    LeftBar,
    RightBar,
    Sliders
  },

  data (){
    return{
      source:""
    }
  },
  methods:{
    sourceChanged: function (source) {
      this.source = source;
      // body...
    }
  }
}



</script>

<style>
#app {
 
}
.h-t{
  background-image: linear-gradient(rgba(0,0,0,0.63),rgba(0,0,0,0.63)),url(https://images.pexels.com/photos/261949/pexels-photo-261949.jpeg?w=940&h=650&auto=compress&cs=tinysrgb);
  height: 340px;
  background-size: cover;
  background-attachment: fixed;
  color: white;
}
.tet{
  font-size: 3.5em;
  font-weight: 400;
  padding-top: 10px;
  font-family: raleway;
}
.tet > b{
  font-weight: 200;
  text-transform: ;
   font-family: raleway;
}
.navbar-default {
    background-color: #fff;
    border-color: #e7e7e7;
    border-radius: 1px;
    box-shadow: 0 2px 15px rgba(0,0,0,0.33);
}
.navbar-default.navbar > li >a {
    color: black;
}
.full {
    width: 100%;    
}
.gap {
  height: 30px;
  width: 100%;
  clear: both;
  display: block;
}
.footer {
    background: #fff;
    height: auto;
    padding-bottom: 30px;
    position: relative;
    width: 100%;
    border-bottom: 1px solid #CCCCCC;
    /* border-top: 1px solid #DDDDDD; */
    box-shadow: 0 1px 10px rgba(0,0,0,0.43);
}
.footer p {
  margin: 0;
}
.footer img {
  max-width: 100%;
}
.footer h3 {
    border-bottom: 1px solid #BAC1C8;
    color: #dab114;
    font-size: 20px;
    font-weight: 400;
    line-height: 27px;
    padding: 40px 0 10px;
    text-transform: uppercase;
}
.footer ul {
  font-size: 13px;
  list-style-type: none;
  margin-left: 0;
  padding-left: 0;
  margin-top: 15px;
  color: #7F8C8D;
}
.footer ul li a {
  padding: 0 0 5px 0;
  display: block;
}
.footer a {
  color: #78828D
}
.supportLi h4 {
  font-size: 20px;
  font-weight: lighter;
  line-height: normal;
  margin-bottom: 0 !important;
  padding-bottom: 0;
}


.newsletter-box {
  overflow: hidden;
}
.bg-gray {
  background-image: -moz-linear-gradient(center bottom, #BBBBBB 0%, #F0F0F0 100%);
  box-shadow: 0 1px 0 #B4B3B3;
}
.social li {
  background: none repeat scroll 0 0 #B5B5B5;
  border: 2px solid #B5B5B5;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -o-border-radius: 50%;
  -ms-border-radius: 50%;
  border-radius: 50%;
  float: left;
  height: 36px;
  line-height: 36px;
  margin: 0 8px 0 0;
  padding: 0;
  text-align: center;
  width: 36px;
  transition: all 0.5s ease 0s;
  -moz-transition: all 0.5s ease 0s;
  -webkit-transition: all 0.5s ease 0s;
  -ms-transition: all 0.5s ease 0s;
  -o-transition: all 0.5s ease 0s;
}
.social li:hover {
  transform: scale(1.15) rotate(360deg);
  -webkit-transform: scale(1.1) rotate(360deg);
  -moz-transform: scale(1.1) rotate(360deg);
  -ms-transform: scale(1.1) rotate(360deg);
  -o-transform: scale(1.1) rotate(360deg);
}
.social li a {
  color: #EDEFF1;
}
.social li:hover {
  border: 2px solid #2c3e50;
  background: #2c3e50;
}
.social li a i {
  font-size: 16px;
  margin: 0 0 0 5px;
  color: #EDEFF1 !important;
}
.footer-bottom {
  background: #E3E3E3;
  border-top: 1px solid #DDDDDD;
  padding-top: 10px;
  padding-bottom: 10px;
}
.footer-bottom p.pull-left {
  padding-top: 6px;
}
.payments {
  font-size: 1.5em; 
}
</style>
