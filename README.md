<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>David Chu's China Bistro</title>

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
    <link rel="stylesheet" href="bootstrap-5.2.0-beta1-dist.zip">
    <link rel="stylesheet" href="CSS2.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>
    
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href='https://fonts.googleapis.com/css?family=Oxygen:400,300,700' rel='stylesheet' type='text/css'>
<link href='https://fonts.googleapis.com/css?family=Lora' rel='stylesheet' type='text/css'>
  <style>
  body {
    font-size: 16px;
    color: #fff;
    background-color: #61122f;
    font-family: 'Oxygen', sans-serif;
  }
  
  /** HEADER **/
  #header-nav {
    background-color: #f6b319;
    border-radius: 0;
    border: 0;
  }
  
  #logo-img {
    background: url('(https://user-images.githubusercontent.com/107862323/176650345-4b9beddc-1f33-4dcb-b952-5912c6004aad.png)
') no-repeat;
    width: 150px;
    height: 150px;
    margin: 10px 15px 10px 0;
  }
  
  .navbar-brand {
    padding-top: 25px;
  }
  .navbar-brand h1 { /* Restaurant name */
    font-family: 'Lora', serif;
    color: #557c3e;
    font-size: 1.5em;
    text-transform: uppercase;
    font-weight: bold;
    text-shadow: 1px 1px 1px #222;
    margin-top: 0;
    margin-bottom: 0;
    line-height: .75;
  }
  .navbar-brand a:hover, .navbar-brand a:focus {
    text-decoration: none;
  }
  .navbar-brand p { /* Kosher cert */
    color: #000;
    text-transform: uppercase;
    font-size: .7em;
    margin-top: 15px;
  }
  .navbar-brand p span { /* Star-K */
    vertical-align: middle;
  }
  
  #nav-list {
    margin-top: 10px;
  }
  #nav-list a {
    color: #951C49;
    text-align: center;
  }
  #nav-list a:hover {
    background: #E7E7E7;
  }
  #nav-list a span {
    font-size: 1.8em;
  }
  
  #phone {
    margin-top: 5px;
  }
  #phone a { /* Phone number */
    text-align: right;
    padding-bottom: 0;
  }
  #phone div { /* We Deliver */
    color: #557c3e;
    text-align: right;
    padding-right: 15px;
  }
  
  .navbar-header button.navbar-toggle, .navbar-header .icon-bar {
    border: 1px solid #61122f;
  }
  .navbar-header button.navbar-toggle {
    clear: both;
    margin-top: -30px;
  }
  /* END HEADER */
  
  /* FOOTER */
  .panel-footer {
    margin-top: 30px;
    padding-top: 35px;
    padding-bottom: 30px;
    background-color: #222;
    border-top: 0;
  }
  .panel-footer div.row {
    margin-bottom: 35px;
  }
  #hours, #address {
    line-height: 2;
  }
  #hours > span, #address > span {
    font-size: 1.3em;
  }
  #address p {
    color: #557c3e;
    font-size: .8em;
    line-height: 1.8;
  }
  #testimonials {
    font-style: italic;
  }
  #testimonials p:nth-child(2) {
    margin-top: 25px;
  }
  /* END FOOTER */
  
  
  
  /* HOME PAGE */
  .container .jumbotron {
    box-shadow: 0 0 50px #3F0C1F;
    border: 2px solid #3F0C1F;
  }
  
  #menu-tile, #specials-tile, #map-tile {
    height: 250px;
    width: 100%;
    margin-bottom: 15px;
    position: relative;
    border: 2px solid #3F0C1F;
    overflow: hidden;
  }
  #menu-tile:hover, #specials-tile:hover, #map-tile:hover {
    box-shadow: 0 1px 5px 1px #cccccc;
  }
  #menu-tile {
    background: url('../images/menu-tile.jpg') no-repeat;
    background-position: center;
  }
  #specials-tile {
    background: url('(https://user-images.githubusercontent.com/107862323/176649920-23b187d5-29e7-4326-a2c1-dbc6cfcbe58f.jpg)
') no-repeat;
    background-position: center;
  }
  #menu-tile span, #specials-tile span, #map-tile span {
    position: absolute;
    bottom: 0;
    right: 0;
    width: 100%;
    text-align: center;
    font-size: 1.6em;
    text-transform: uppercase;
    background-color: #000;
    color: #fff;
    opacity: .8;
  }
  /* END HOME PAGE */
  
  /* MENU CATEGORIES PAGE */
  .category-tile { 
    position: relative;
    border: 2px solid #3F0C1F;
    overflow: hidden;
    width: 200px;
    height: 200px;
    margin: 0 auto 15px;
  }
  .category-tile span {
    position: absolute;
    bottom: 0;
    right: 0;
    width: 100%;
    text-align: center;
    font-size: 1.2em;
    text-transform: uppercase;
    background-color: #000;
    color: #fff;
    opacity: .8;
  }
  .category-tile:hover {
    box-shadow: 0 1px 5px 1px #cccccc;
  }
  
  #menu-categories-title + div {
    margin-bottom: 50px;
  }
  /* END MENU CATEGORIES PAGE */
  
  /* SINGLE CATEGORY PAGE */
  .menu-item-tile {
    margin-bottom: 25px;
  }
  .menu-item-tile hr {
    width: 80%;
  }
  .menu-item-tile .menu-item-price {
    font-size: 1.1em;
    text-align: right;
    margin-top: -15px;
    margin-right: -15px;
  }
  .menu-item-tile .menu-item-price span {
    font-size: .6em;
  }
  .menu-item-photo {
    position: relative;
    border: 2px solid #3F0C1F; 
    overflow: hidden;
    padding: 0;
    margin-right: -15px;
    margin-left: auto;
    margin-bottom: 20px;
    max-width: 250px;
  }
  .menu-item-photo div {
    position: absolute;
    bottom: 0;
    right: 0;
    width: 80px;
    background-color: #557c3e;
    text-align: center;
  }
  .menu-item-description {
    padding-right: 30px;
  }
  h3.menu-item-title {
    margin: 0 0 10px;
  }
  .menu-item-details {
    font-size: .9em;
    font-style: italic;
  }
  /* END SINGLE CATEGORY PAGE */
  
  
  /********** Large devices only **********/
  @media (min-width: 1200px) {
    .container .jumbotron {
      background: url('(https://user-images.githubusercontent.com/107862323/176649362-a491aa3b-da25-4f24-b79a-f9c9bc2f0580.jpg)
') no-repeat;
      height: 675px;
    }
  }
  
  /********** Medium devices only **********/
  @media (min-width: 992px) and (max-width: 1199px) {
    /* Header */
    #logo-img {
      background: url('(https://user-images.githubusercontent.com/107862323/176649630-9aad3ee7-fe14-4fb3-b4a1-d76bd63800d0.png)
') no-repeat;
      width: 100px;
      height: 100px;
      margin: 5px 5px 5px 0;
    }
    /* End Header */
  
    /* Home Page */
    .container .jumbotron {
      background: url('(https://user-images.githubusercontent.com/107862323/176648342-743e7a4a-8b42-45ae-8882-e63feb7a72a0.jpg)
') no-repeat;
      height: 558px;
    }
    /* End Home Page */
  }
  
  /********** Small devices only **********/
  @media (min-width: 768px) and (max-width: 991px) {
    /* Home Page */
    .container .jumbotron {
      background: url('(https://raw.githubusercontent.com/kvmallik/assignment-5/main/IMAGES/jumbotron_768.jpg') no-repeat;
      height: 432px;
    }
    /* End Home Page */
  }
  
  /********** Extra small devices only **********/
  @media (max-width: 767px) {
    /* Header */
    .navbar-brand {
      padding-top: 10px;
      height: 80px;
    }
    .navbar-brand h1 { /* Restaurant name */
      padding-top: 10px;
      font-size: 5vw; /* 1vw = 1% of viewport width */
    }
    .navbar-brand p { /* Kosher cert */
      font-size: .6em;
      margin-top: 12px;
    }
    .navbar-brand p img { /* Star-K */
      height: 20px;
    }
  
    #collapsable-nav a { /* Collapsed nav menu text */
      font-size: 1.2em;
    }
    #collapsable-nav a span { /* Collapsed nav menu glyph */
      font-size: 1em;
      margin-right: 5px;
    }
  
    #call-btn > a {
      font-size: 1.5em;
      display: block;
      margin: 0 20px;
      padding: 10px;
      border: 2px solid #fff;
      background-color: #f6b319;
      color: #951c49;
    }
    #xs-deliver {
      margin-top: 5px;
      font-size: .7em;
      letter-spacing: .1em;
      text-transform: uppercase;
    }
    /* End Header */
  
    /* Footer */
    .panel-footer section {
      margin-bottom: 30px;
      text-align: center;
    }
    .panel-footer section:nth-child(3) {
      margin-bottom: 0; /* margin already exists on the whole row */
    }
    .panel-footer section hr {
      width: 50%;
    }
    /* End Footer */
  
    /* Home Page */
    .container .jumbotron {
      margin-top: 30px;
      padding: 0;
    }
    #menu-tile, #specials-tile {
      width: 360px;
      margin: 0 auto 15px;
    }
  
    .menu-item-photo {
      margin-right: auto;
    }
    .menu-item-tile .menu-item-price {
      text-align: center;
    }
    .menu-item-description {
      text-align: center;;
    }
  }
  
  
  /********** Super extra small devices Only :-) (e.g., iPhone 4) **********/
  @media (max-width: 479px) {
    /* Header */
    .navbar-brand h1 { /* Restaurant name */
      padding-top: 5px;
      font-size: 6vw;
    }
    /* End Header */
    
    /* Home page */
    #menu-tile, #specials-tile {
      width: 280px;
      margin: 0 auto 15px;
    }
  
    .col-xxs-12 {
      position: relative;
      min-height: 1px;
      padding-right: 15px;
      padding-left: 15px;
      float: left;
      width: 100%;
    }
  }
  </style>
</head>
<body>
    <header>
        <nav id="header-nav" class="navbar navbar-default">
          <div class="container">
            <div class="navbar-header">
                <a href="index.html" class="pull-left visible-md visible-lg">
                  <div id="logo-img" alt="Logo image"></div>
                </a>

                <div class="navbar-brand">
                    <a href="index.html"><h1>David Chu's China Bistro</h1></a>
                    <p>
                      <img src="images/star-k-logo.png" alt="Kosher certification">
                      <span>Kosher Certified</span>
                    </p>
                </div>

                <button id="navbarToggle" type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#collapsable-nav" aria-expanded="false">
                    <span class="sr-only">Toggle navigation</span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                  </button>
                </div>
                
                <div id="collapsable-nav" class="collapse navbar-collapse">
                  <ul id="nav-list" class="nav navbar-nav navbar-right">
                   <li id="navHomeButton" class="visible-xs active">
                     <a href="index.html">
                       <span class="glyphicon glyphicon-home"></span> Home</a>
                   </li>
                   <li id="navMenuButton">
                     <a href="menu-categories.html" onclick="$dc.loadMenuCategories();">
                       <span class="glyphicon glyphicon-cutlery"></span><br class="hidden-xs"> Menu</a>
                   </li>
                   <li>
                     <a href="#">
                       <span class="glyphicon glyphicon-info-sign"></span><br class="hidden-xs"> About</a>
                   </li>
                   <li>
                     <a href="#">
                       <span class="glyphicon glyphicon-certificate"></span><br class="hidden-xs"> Awards</a>
                   </li>
                   <li id="phone" class="hidden-xs">
                     <a href="tel:410-602-5008">
                       <span>410-602-5008</span></a><div>* We Deliver</div>
                   </li>
                  </ul><!-- #nav-list -->
                </div><!-- .collapse .navbar-collapse -->
          </div>
        </nav>
    </header>

    <div id="call-btn" class="visible-xs">
      <a class="btn" href="tel:410-602-5008">
      <span class="glyphicon glyphicon-earphone"></span>
      410-602-5008
      </a>
    </div>
    <div id="xs-deliver" class="text-center visible-xs">* We Deliver</div>

   
  
    <div id="main-content" class="container">
      <div class="jumbotron">
        <img src="D:\IMAGES\jumbotron_768.jpg" alt="picture of restarunt" class="img-responsive visible-xs">
      </div>
        <div id="home-tiles" class="row">
          <div class="col-md-4 col-sm-6 col-xs-12">
            <a href="menu-categories.html"><div id="menu-tile"><span>menu</span></div></a>
            </div>
            <div class="col-md-4 col-sm-6 col-xs-12">
              <a href="single-categories.html"><div id="specials-tile"><span>specials</span></div></a>
              </div>
              <div class="col-md-4 col-sm-12 col-xs-12">
                  <a href="https://goo.gl/maps/DsSgRPt3gSG53Vpb9" target="_blank">
                    <div id="map-tile">
                      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3084.6752464097885!2d-76.71388214998836!3d39.36359027940089!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c81a14e7817803%3A0xab20a0e99daa17ea!2sDavid%20Chu&#39;s%20China%20Bistro!5e0!3m2!1sen!2sin!4v1656171700875!5m2!1sen!2sin" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                      <span>map</span>
                    </div>
                  </a>
              </div>
              </div>
    </div>
  
    <footer class="panel-footer">
      <div class="container">
        <div class="row">
          <section id="hours" class="col-sm-4">
            <span>Hours:</span><br>
            Sun-Thurs: 11:15am - 10:00pm<br>
            Fri: 11:15am - 2:30pm<br>
            Saturday Closed
            <hr class="visible-xs">
          </section>
          <section id="address" class="col-sm-4">
            <span>Address:</span><br>
            7105 Reisterstown Road<br>
            Baltimore, MD 21215
            <p>* Delivery area within 3-4 miles, with minimum order of $20 plus $3 charge for all deliveries.</p>
            <hr class="visible-xs">
          </section>
          <section id="testimonials" class="col-sm-4">
            <p>"The best Chinese restaurant I've been to! And that's saying a lot, since I've been to many!"</p>
            <p>"Amazing food! Great service! Couldn't ask for more! I'll be back again and again!"</p>
          </section>
        </div>
        <div class="text-center">&copy; Copyright David Chu's China Bistro 2016</div>
      </div>
    </footer>
  



    <!-- jQuery (Bootstrap JS plugins depend on it) -->
   <script src="js/jquery-3.6.0.js"></script>
   <script src="js/bootstrap.min.js"></script>
   <script src="js/ajax-utils.js"></script>
   <script src="js/script.js"></script>
</body>
</html>
