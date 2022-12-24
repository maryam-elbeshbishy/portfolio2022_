<template>
  <div class="container-3">
    <div class="item-1">
      <div>
        <img src="..\img\pfp.jpg" style="width:20vw; border-radius: 10px;display: block; margin-top: 4vh;margin-left: auto; margin-right: auto;" alt="ART NOT LOADED">
      </div>
      <div class="welcome" style="font-size: 3.5rem; width:45vh; background-color: #f3e2d2; color:#56131a;">
        Thats Me!
      </div>
      <div class="btn">
        <q-btn class="button" color="button_icon-1" style="width:45%;font-size: 3.5vh;font-weight: 600" href="https://www.linkedin.com/in/melbeshb/" label="LinkedIn" />
        <q-btn class="button" color="button_icon-1" style="width:45%;font-size: 3.5vh;font-weight: 600" href="https://github.com/maryam-elbeshbishy" label="GitHub" />
      </div>
      <div class="btn">
        <q-btn class="button" color="button_icon-1" style="width:45%;font-size: 3.5vh;font-weight: 600" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Resume" />
        <q-btn class="button" color="button_icon-1" style="width:45%;font-size: 3.5vh;font-weight: 600" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Email" />
      </div>
    </div>
    
    <div class="item-2">
      <div>
        <q-btn class="nav_button" color="button_nav-1" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="Home" to="/"/>
        <q-btn class="nav_button" color="button_nav-1" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="Projects" to="/projects"/>
        <q-btn class="nav_button" color="button_nav-1" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="Art Portfolio" to="/art"/>
        <q-btn class="nav_button" color="button_nav-1" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="DevLogs" to="/devlogs"/>
      </div>
      
      <div class="name" style="background-color:#b58d58 ;color:#2a1801">
        <p color="white" style="font-family:'Playfair Display'; font-size:2rem ">A Little About Me...</p>
        <p color="white" style="font-weight:600; font-family:'Dosis'; sans-serif; font-size:2em">
        Tech Related
      </p>
        <p color="white" style="font-weight:600; font-family:'Dosis'; sans-serif; font-size:1.5em">
        Currently, my biggest passion is learning about <b>virtual reality</b>, which the driving force in me taking the leap to 
        <b>learn unity and C# through</b>> a course held by Circuit Stream, to learn how to <b>create XR experiences</b>, ranging from AR mobile applications to creating
        a simple game in VR
        <br>
        Along with that, I am quite passionate about learning more technologies related to Data Science. After having learnt many libraries that 
        are useful in Python, I would like to learn technologies that deal with big data!
        </p>

        <p color="white" style="font-weight:600; font-family:'Dosis'; sans-serif; font-size:2em">
        Hobbies
      </p>
        <p color="white" style="font-weight:600; font-family:'Dosis'; sans-serif; font-size:1.5em">
        Recently, I've picked up many hobbies that I feel fullfill my life and ultimately help regulate my attention span. These hobbies include <b>drawing</b>> (mainly 
        digital, using procreate), <b>reading, playing piano and solving rubicks cubes</b>! Playing piano would have to be my favorite hobby at the moment, since it has 
        been a life long dream, and after a few years of contemplating whether it was worth I've decided to self teach myself!  
        <br>
        Fun fact: My lowest time to solve a standard rubicks cube is ~41sec! 
        </p>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
.bg-button_icon-1 {
  background: #762f38 !important;
}
.bg-button_nav-1 {
  background: #6b481a !important;
}
.container-3 {
  display: flex; /* create a flex container */
  /*have the div span the whole screen + change background color */
  position:fixed;
  width:100%;
  height:100%;
  /*changes all text to white*/
  color:rgb(212, 212, 212);
  background-color: rgb(38, 0, 6);
}

.item-1 {
  flex: 1; /* 1/3 of the container's width */
  margin: 2vw;
  
  
}

.item-2 {
  flex: 2; /* 2/3 of the container's width */
  margin: 2vw;
}
</style>