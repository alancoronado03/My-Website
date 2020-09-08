<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
</head>
<body>
    <style>* {box-sizing: border-box}

        /* Set height of body and the document to 100% */
        body, html {
          height: 100%;
          margin: 0;
          font-family: Arial;
        }
        
        /* Style tab links */
        .tablink {
          background-color: #555;
          color: white;
          float: left;
          border: none;
          outline: none;
          cursor: pointer;
          padding: 14px 16px;
          font-size: 40px;
          width: 33.3%;
        }
        
        .tablink:hover {
          background-color: #000000;
        }
        
        /* Style the tab content (and add height:100% for full page content) */
        .tabcontent {
         color: white;
          display: none;
          padding: 100px 20px;
          height: 100%;
        }
        h1{
          position: relative;
          text-align: center;
         
        }
        center{
          display:block;
          margin-left: auto;
          margin-right: auto;
          width: 50%;
          
        
        }
        
        
          
        
        
        
        
        
        #Home {background-color: crimson ;}
        #Portfolio {background-color:olive;}
        #AboutMe {background-color: blueviolet;}
</style>

 <button class="tablink" onclick="openPage('Home', this, 'black')" id="defaultOpen">Home</button>
 <button class="tablink" onclick="openPage('Portfolio', this, 'black')">Portfolio</button>
 <button class="tablink" onclick="openPage('AboutMe', this, 'black')">About Me</button>


 <div id="Home" class="tabcontent">
  <h1>This is Alan Coronado's Home Page!!!</h1>
  <h2>This is my home away from home:</h2>
  <img src="images/Soccerfield.jpg" alt="Soccer Field" class="center">
 </div>

 <div id="Portfolio" class="tabcontent">
  <h1>Below you can see some of my Assigments:</h1>
  
 
 </div>

 <div id="AboutMe" class="tabcontent">
  <h1>Here is a little background information about myself: </h1>
  <img  src="images/map.gdl.jpg" alt="Guadalajara" class="center">
  <p>"This is where I am from"</p>

 </div>
<script>function openPage(pageName,elmnt,color) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
      tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablink");
    for (i = 0; i < tablinks.length; i++) {
      tablinks[i].style.backgroundColor = "";
    }
    document.getElementById(pageName).style.display = "block";
    elmnt.style.backgroundColor = color;
  }
  
  
  
  // Get the element with id="defaultOpen" and click on it
  document.getElementById("defaultOpen").click();
  </script>

   
</body>
</html> 
