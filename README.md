# CODE2132-2023

GH to ThreeJS working files


Guide to WEB>GH>WEB:
<br>

Project structure:
- YourProjectDirectory
    - public
        - index.html
        - app.js
    - server.js
    - input.json

Install Required Packages (in terminal, make to CD into 'YourProjectDirectory'): <br>
"npm init -y" - this command will tell you which directory you are in<br>
"npm install express"<br>
"node server.js"


    .bar1, .bar2, .bar3 {
    width: 35px;
    height: 5px;
    background-color: #F5F5F4;
    margin: 6px 0;
    transition: 0.4s;
   } 
   .change .bar1 {
    transform: translate(0, 11px) rotate(-45deg);
   } 
.change .bar2 {
  opacity: 0;
}
 .change .bar3 {
  transform: translate(0, -11px) rotate(45deg);
  }

  .menu-container {
  display: inline-block;
  cursor: pointer;
  left: 10px;
  position: absolute;
  top: 10px;
  z-index: 5000;
 } 

 .overlay {
  top: 0;
  height: 90%;
  width: 0;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: rgb(0,0,0);
  background-color: rgba(0,0,0, 0.9);
  overflow-x: hidden;
  transition: 0.5s;
}

 .NavControl .overlay {
  width: 0%;
 }

.overlay-content {
  position: relative;
  top: 25%;
  width: 100%;
  text-align: center;
  margin-top: 30px;
}

.overlay a {
  padding: 8px;
  text-decoration: none;
  font-size: 36px;
  color: #818181;
  display: block;
  transition: 0.3s;
}

.overlay a:hover, .overlay a:focus {
  color: #f1f1f1;
}

.overlay .closebtn {
  position: absolute;
  top: 10px;
  left: 10px;
}

@media screen and (max-height: 450px) {
  .overlay a {font-size: 20px}
  .overlay .closebtn {
  font-size: 40px;
  top: 15px;
  right: 35px;
  }
}

 <div id="myNav" class="overlay" >
    <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>
    <div class="overlay-content">
      <a href="#" >About</a>
      <a href="#">Services</a>
      <a href="#">Clients</a>
      <a href="#">Contact</a>
    </div>
  </div>


  <div class="menu-container" onclick="myFunction(this);openNav()">
      <div class="bar1"></div>
      <div class="bar2"></div>
      <div class="bar3"></div>
    </div>

    <script> //menu scripts
  function openNav() {

   
    if (document.getElementById("myNav").style.width <= "1%")
    {

      document.getElementById("myNav").style.width = "20%";

    }
   
    
  }
  
  function closeNav() {
   
    document.getElementById("myNav").style.width = "0%";
    
  }
  </script>

<script> //button script
  function myFunction(x) {
    x.classList.toggle("change");
  }

  function navFunction(x){
    x.classList.toggle("NavControl");
  }
  </script>
