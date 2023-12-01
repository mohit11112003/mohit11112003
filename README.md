
<!doctype html>
<html lang="en">

<head>
  <script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
  <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
  <link rel="stylesheet" href="resp-style.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link rel="stylesheet" href="style.css">
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Hotel Management</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-iYQeCzEYFbKjA/T2uDLTpkwGzCiq6soy8tYaI1GyVh/UjpbCx/TYkiZhlZB6+fzT" crossorigin="anonymous">
  <style>
    @media screen and (max-width: 720px) {
      #availibility {
        display: flex;
        flex-direction: column;
        height: 37vh;
        /* background-color: red; */
        margin-bottom: 5vh;
      }

      .rooms {
        flex-direction: column;
        height: 142vh;
      }

      #descroom {
        height: 4vh;
      }

      #gallary {
        margin-top: 14vh;
      }

      #room2 {
        display: flex;
        margin-top: -4vh;
        /* flex-direction: column-reverse; */
      }

      #roomimg2 {
        margin-top: -4vh;
      }

      #services {
        flex-direction: column;
      }

      #card {
        width: 85vw;
      }

      #seegallary {
        margin-top: 10vh;
        font-size: 2rem;
      }

      #gallimg {
        width: 99vw;
      }

      .staffcon {
        flex-direction: column;
      }
     
    }


    @media screen and (max-width: 370px) {
      #availibility {
        display: flex;
        flex-direction: column;
        height: 36vh;
        /* background-color: red; */
        margin-bottom: 5vh;
      }

      .rooms {
        flex-direction: column;
        height: 140vh;
      }

      #descroom {
        height: 4vh;
      }

      #gallary {
        margin-top: 12vh;
      }

      #room2 {
        display: flex;
        margin-top: -4vh;
        /* flex-direction: column-reverse; */
      }

      #roomimg2 {
        margin-top: -4vh;
      }

      #services {
        flex-direction: column;
      }

      #card {
        width: 85vw;
      }

      #seegallary {
        margin-top: 10vh;
        font-size: 2rem;
      }

      #gallimg {
        width: 99vw;
      }

      .staffcon {
        flex-direction: column;
      }

      #team {
        margin-top: -7vh;
      }
    }

    @media screen and (min-width:450px) {

      .scroll-down::after,
      .scroll-down::before {
        margin-left: 35.75vw;
      }
    }

    @media screen and (min-width:800px) {

      .scroll-down::after,
      .scroll-down::before {
        margin-left: 37.75vw;
      }
    }

    @media screen and (min-width:1200px) {

      .scroll-down::after,
      .scroll-down::before {
        margin-left: 36.55vw;
      }
    }
  </style>
</head>

<body>
  <!-- navbar code starts  -->
  
 
  <div class="container-fluid" id="navcon">
    <nav id="navbar" class="navbar navbar-dark bg-dark fixed-top">
      <div class="container-fluid">
        <img src="/img/images.jpg" class="img-fluid" alt="logo" id="logo">
        <!--book  button   -->
        <li class="nav-item mt-3 mt-lg-0">
          <a class="main-btn" href="#">Book Now</a>
        </li>

       

        

        <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasDarkNavbar"
          aria-controls="offcanvasDarkNavbar">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="offcanvas offcanvas-end text-bg-dark" tabindex="-1" id="offcanvasDarkNavbar"
          aria-labelledby="offcanvasDarkNavbarLabel">
          <div class="offcanvas-header">
            <h5 class="offcanvas-title" id="offcanvasDarkNavbarLabel">Welcome To Taj Hotel</h5>


            <button type="button" class="btn-close btn-close-white" data-bs-dismiss="offcanvas"
              aria-label="Close"></button>
          </div>
          <div class="offcanvas-header">
            <h6>Founder:Kunti</h6>
          </div>
          <div class="offcanvas-body">
            <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
              <li class="nav-item">
                <a aria-current='page' class='nav-link active' href='/'>Home</a>
              </li>
              <li class="nav-item">
                <a class='nav-link' href='/about'>About</a>
              </li>
              <li class="nav-item">
                <a class='nav-link' href='/team'>Team</a>
              </li>
              <li class="nav-item">
                <a class='nav-link' href='/room'>Rooms</a>
              </li>
              <li class="nav-item">
                <a class='nav-link' href='/service'>Services</a>
              </li>
              <li class="nav-item">
                <a class='nav-link' href='/contact'>Contact Us</a>
              </li>
            

            </ul>
            <form class="d-flex" role="search">
              <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
              <button class="btn btn-success" type="submit">Search</button>
            </form>
          </div>
        </div>
      </div>
    </nav>
  </div>



  <!-- bg rooms pic  -->



  <div class="container-fluid" id="navcon">
    <div id="carouselExampleFade" class="carousel slide carousel-fade" data-bs-ride="carousel">
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="/img/bgroom6 (1).jpg" class="bg-fit" alt="Hotel Img">



          <div class="carousel-caption  ">
            <h1 id="imgtext" data-aos="slide-up" data-aos-offset="10">Welcome To Taj Hotel</h1>

          </div>


        </div>
      </div>

    </div>

  </div>
  </div>
  <!-- bg ends  -->




  <!-- check availability code  -->
  <div class="bgcheck">
    <div class="check">
      <h2 style="text-align: center; font-size: 3rem;" data-aos="slide-down">Check Availability</h2>
    </div>

    <div class="container" id="availibility" data-aos="zoom-in">
      <ul class="nav justify-content-center " style="margin-top: .8rem;">

        <li class="nav-item" style="margin-top: 1rem;">
          <label>Check-In</label>
          <a class="nav-link active" aria-current="page"><input style="padding: 12px;" type="date"></a>

        </li>
        <li class="nav-item" style="margin-top: 1rem;">
          <label>Check-Out</label>
          <a class="nav-link active" aria-current="page"><input style="padding: 12px;" type="date"></a>
        </li>
        <li class="nav-item" style="margin-top: 3rem;">
          <label>No.of Person</label>

          <a class="nav-link"><select>
              <option value="--select--">--person--</option>
              <option value="1">1</option>
              <option value="2">2</option>
              <option value="3">3</option>
              <option value="4">4</option>
              <option value="5">5</option>

            </select></a>
        </li>



        <li class="nav-item mt-3 mt-lg-0">
          <a class="av-btn" style="padding: 12px; margin-top: 2.3rem;">CHECK AVAILABILITY</a>
        </li>

      </ul>
    </div>
  </div>

  <!-- our rooms code starts  -->

  <div class="check" id="gallary">
    <h2 style="text-align: center; font-size: 4.5rem;" data-aos="zoom-in-right"> Rooms </h2>
  </div>

  <!-- room img and desc code   -->
  <div class="roomcon" id="prices" >
    <div class="rooms">
      <span id="roomimg">
        <img src="/img/room1 (2).jpg" class="img-fluid" alt="..." data-aos="zoom-in">
      </span>
      <span id="descroom">
        <span>
          <h2 id="price">&#8377; 4999<span id="day">/day</span></h2>
          <h2 style="margin: 5vh 0 5vh 0;">Superior Room</h2>
          <h4 style="margin: 5vh 0 12vh 0;">All our guestrooms are elegantly furnished with handmade furniture include
            luxury en-suite facilities with complimentary amenities pack, flat screen LCD TV, tea/coffee making
            facilities, fan, hairdryer and the finest pure white linen and towels.</h4>
          <li class="nav-item mt-3 mt-lg-0" id="bookbtn">
            <a class="main-btn" href="#" data-aos="zoom-in">Book Now</a>
          </li>

        </span>
      </span>
    </div>
    <!-- text of deluxe room  -->
    <div class="check" id="gallary">
      <h2 style="text-align: center; font-size: 4rem;" data-aos="zoom-in">Deluxe Room </h2>
    </div>



    <!-- only check  -->
    <!-- room img and desc code   -->
    <div class="roomcon" id="prices">
      <div class="rooms">
        <span id="roomimg">
          <img src="/img/room1 (3).jpg" class="img-fluid" alt="..." data-aos="zoom-in">
        </span>
        <span id="descroom">
          <span>
            <h2 id="price">&#8377; 3249<span id="day">/day</span></h2>
            <h2 style="margin: 5vh 0 5vh 0;">Deluxe Room</h2>
            <h4 style="margin: 5vh 0 12vh 0;">Enjoy our elegant 40 m² guest rooms, designed in warm beige tones and
              tailored to the needs of private and business travelers alike.

              All rooms have a large marble bathroom, a double bed, air conditioning, an additional work area with free
              internet access and a walk-in closet.

              Our superior rooms impress with a wonderful view of the city and the adjacent park.</h4>
            <li class="nav-item mt-3 mt-lg-0" id="bookbtn">
              <a class="main-btn" href="#" data-aos="zoom-in">Book Now</a>
            </li>

          </span>
        </span>
      </div>

      <!-- check ends  -->



      <!-- text of twin room  -->
      <div class="check" id="gallary">
        <h2 style="text-align: center; font-size: 4rem;" data-aos="zoom-in">Twin Room </h2>
      </div>

      <!-- third room code  -->
      <div class="rooms">
        <span id="roomimg">
          <img src="/img/room1 (1).jpg" class="img-fluid" alt="..." data-aos="zoom-in">
        </span>
        <span id="descroom">
          <span>
            <h2 id="price">&#8377; 1999<span id="day">/day</span></h2>
            <h2 style="margin: 5vh 0 5vh 0;">Twin Room</h2>
            <h4 style="margin: 5vh 0 12vh 0;">All our guestrooms are elegantly furnished with handmade furniture include
              luxury en-suite facilities with complimentary amenities pack, flat screen LCD TV, tea/coffee making
              facilities, fan, hairdryer and the finest pure white linen and towels.</h4>
            <li class="nav-item mt-3 mt-lg-0" id="bookbtn">
              <a class="main-btn" href="#" data-aos="zoom-in">Book Now</a>
            </li>

          </span>
        </span>
      </div>

      <!-- text of duplex room  -->
      <div class="check" id="gallary">
        <h2 style="text-align: center; font-size: 4rem;" data-aos="zoom-in-right">Duplex Room </h2>
      </div>


      <!-- four check  -->
      <!-- room img and desc code   -->
      <div class="roomcon" id="prices">
        <div class="rooms">
          <span id="roomimg">
            <img src="/img/bgroom4.jpg" class="img-fluid" alt="..." data-aos="zoom-in">
          </span>
          <span id="descroom">
            <span>
              <h2 id="price">&#8377; 1449<span id="day">/day</span></h2>
              <h2 style="margin: 5vh 0 5vh 0;">Duplex Room</h2>
              <h4 style="margin: 5vh 0 12vh 0;">A duplex is a multi-family home that has two units in the same building.
                These two units always share a common wall, but the floor plan can vary. Units can be arranged either
                side
                by side or stacked on top of one another, each occupying an entire floor or two of the building.</h4>
              <li class="nav-item mt-3 mt-lg-0" id="bookbtn">
                <a class="main-btn" href="#" data-aos="zoom-in">Book Now</a>
              </li>

            </span>
          </span>
        </div>

        <!-- four room code  -->

        <!-- <div class="rooms">

      

   servicesss  -->
        <div class="services" id="services">
          <h2 data-aos="zoom-out">Our Services</h2>
        </div>


        <!-- services card starts  -->
        <div class="staffcon" id="services">
          <div class="card" id="card">
            <img src="/img/wifi.jpg" class="card-img-top" alt="..." id="staff">
            <div class="card-body" id="staffcard">
              <h5 class="card-title text-center">Full Speed of Wifi</h5>
            </div>
          </div>

          <div class="card" id="card">
            <img src="/img/food.jpg" class="card-img-top" alt="..." id="staff">
            <div class="card-body" id="staffcard">
              <h5 class="card-title text-center">24x7 Food Services</h5>
            </div>
          </div>

          <div class="card" id="card">
            <img src="/img/parking.jpg" class="card-img-top" alt="..." id="staff">
            <div class="card-body" id="staffcard">
              <h5 class="card-title text-center">Free Safe Parking</h5>
            </div>
          </div>
        </div>

        <!-- services ends  -->




        <!-- see the gallary code  -->
        <div class="check" id="gallary">
          <h2 id="seegallary" style="text-align: center; font-size: 4rem;" data-aos="zoom-in-right">See the gallary
          </h2>
        </div>

        <!-- gallary img code  -->
        <div class="gallarycon">
          <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="true" id="navcon">
            <div class="carousel-indicators">
              <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"
                aria-current="true" aria-label="Slide 1"></button>
              <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
                aria-label="Slide 2"></button>
              <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
                aria-label="Slide 3"></button>
            </div>
            <div class="carousel-inner">
              <div class="carousel-item active">
                <img src="/img/foodimg1.jpg" class="d-block " alt="Img" id="gallimg">
              </div>
              <div class="carousel-item">
                <img src="/img/staff1.jpg" class="d-block" alt="Img" id="gallimg">
              </div>
              <!-- <div class="carousel-item">
                <img src="/img/bgroom5.jpg" class="d-block " alt="Img" id="gallimg">
              </div> -->

              <!-- food img  -->
              <div class="carousel-item">
                <img src="/img/foodimg.jpg" class="d-block " alt="Img" id="gallimg">
              </div>
              <div class="carousel-item">
                <img src="/img/foodimg1.jpg" class="d-block " alt="Img" id="gallimg">
              </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators"
              data-bs-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators"
              data-bs-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
          </div>
        </div>

        <!-- ends  -->

        <!-- about us page  -->
        <div class="services" id="about">
          <h2 data-aos="zoom-out">About Us</h2>
        </div>
        <div class="container mt-5" style="background-color: black; color:white;">
          <h5 class="text-center">Since:1947</h5>
          <h3 style="color: yellow;">“Customers may forget what you said but they will never forget how you made them
            feel”.</h3>
          <h3>Our Team is fully dedicated. We never want that you will disappointed with our services</h3>
          <h4 style="color: yellow;">Quick action:+91 1100 200 100</h4>
          <img src="/img/staff1.jpg" class="d-block " alt="Img" id="gallimg">


        </div>





        <div class="check" id="team">
          <h2 style="text-align: center; font-size: 2.8rem; margin-top: 15vh;" data-aos="zoom-in">Our Special Staff</h2>
        </div>




        <!-- our staff code starts  -->
        <div class="staffcon">
          <div class="card" id="card">
            <img src="/img/staffhead1.jpg" class="card-img-top" alt="..." id="staff">
            <div class="card-body" id="staffcard">
              <h5 class="card-title">Mr.Yogesh Baghel</h5>
              <p class="card-text">Manager</p>
            </div>
          </div>

          <div class="card" id="card">
            <img src="/img/staffhead2.jpg" class="card-img-top" alt="..." id="staff">
            <div class="card-body" id="staffcard">
              <h5 class="card-title">Mr. Abhay Pratap</h5>
              <p class="card-text">Chief Reciption Officer</p>
            </div>
          </div>

          <div class="card" id="card">
            <img src="/img/chef.jpg" class="card-img-top" alt="..." id="staff">
            <div class="card-body" id="staffcard">
              <h5 class="card-title">Mr. Raj Kumar</h5>
              <p class="card-text">Master Chef</p>
            </div>
          </div>
        </div>

        <!-- footer  -->
        <div class="footercon">
          <h5>Name: Kunti </h5>
          <p>Project: Hotel Management Website</p>
          <p>Phone Support:+91-1100 200 100</p>
          <h6>&copy; All Rights Reserved</h6>
        </div>


        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/js/bootstrap.bundle.min.js"
          integrity="sha384-u1OknCvxWvY5kfmNBILK2hRnQC3Pr17a+RTT6rIHI7NnikvbZlHgTPOOmMi466C8"
          crossorigin="anonymous"></script>

        <!-- our aos data  -->
        <script src="https://unpkg.com/aos@next/dist/aos.js"></script>
        <script>
          AOS.init({
            offset: 240,
            duration: 1000
          });
        </script>




</body>

</html>- 👋 Hi, I’m @mohit11112003
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mohit11112003/mohit11112003 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
