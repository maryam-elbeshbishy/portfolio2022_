<template>
  <div class="container">
    <div class="item-1">
      <div>
        <img src="..\img\TL.jpg" style="width:27vw; border-radius: 10px;display: block;margin-left: auto; margin-right: auto;" alt="ART NOT LOADED">
      </div>
      <div class="welcome">
        Welcome to my corner of the internet!
      </div>

      <!-- BUTTONS FOR SOCIALS -->
      <div class="btn">
        <q-btn class="button" color="button_icon" style="width:20%;font-size: 3.5vh;font-weight: 600" href="https://www.linkedin.com/in/melbeshb/" label="Img" />
        <q-btn class="button" color="button_col" text-color="white" style="font-weight: 600; width:70%; font-size: 3.5vh;" href="https://www.linkedin.com/in/melbeshb/" label="LinkedIn" /> 
      </div>

      <div class="btn">
        <q-btn class="button" color="button_icon" style="width:20%;font-size: 3.5vh;font-weight: 600" href="https://github.com/maryam-elbeshbishy" label="Img" />
        <q-btn class="button" color="button_col" text-color="white" style="font-weight: 600; width:70%; font-size: 3.5vh;" href="https://github.com/maryam-elbeshbishy" label="GitHub" />
      </div>

      <div class="btn">
        <q-btn class="button" color="button_icon" style="width:20%;font-size: 3.5vh;font-weight: 600" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Img" />
        <q-btn class="button" color="button_col" text-color="white" style="font-weight: 600; width:70%; font-size: 3.5vh;" href="mailto: maryam.elbeshbishy@ryerson.ca" label="GitHub" />
      </div>

      <!-- HAVE TO CHANGE THE HREF TO GO TO A PDF OF RESUME -->
      <div class="btn">
        <q-btn class="button" color="button_icon" style="width:20%;font-size: 3.5vh;font-weight: 600" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Img" />
        <q-btn class="button" color="button_col" text-color="white" style="font-weight: 600; width:70%; font-size: 3.5vh;" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Resume" />
      </div>

    </div>

    <div class="item-2">
      <div>
        <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="About Me" to="/about"/>
        <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="Projects" to="/projects"/>
        <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="Art Portfolio" to="/art"/>
        <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:24%; font-size: 1.8em;" label="DevLogs" to="/devlogs"/>
      </div>
      <div class="name">
        <p color="white" style="font-family:'Playfair Display'; font-size:4rem ">Maryam Elbeshbishy</p>
        <p color="white" style="font-weight:600; font-family:'Dosis'; sans-serif; font-size:2em ">Computer Science - Toronto Metropolitan University</p>
        <p color="white" style="font-weight:600; font-family:'Dosis'; sans-serif; font-size:1.5em">Hi! As you may have seen my name is Maryam, Im currently working as a Research Assistant
        at Ryerson University, I am quite passionate about Data Science and XR Development, currently taking courses in both to expand my knowledge! Check the rest of my website for more
      information. <br> PS. Any art on this website was created by me!</p>
      </div>
      <div>
        <img src="..\img\Img_BR.jpg" style="width:57vw; border-radius: 10px;display: block;margin-left: auto; margin-right: auto;" alt="ART NOT LOADED">
      </div>
    </div>
</div>

</template>

<script>

</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Dosis:wght@400;600;800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Dosis&family=Playfair+Display:wght@600&display=swap');

/*quasar specified colors*/
.bg-button_col {
  background: #d57962 !important;
}
.bg-button_icon {
  background: #7aa78a !important;
}
.bg-button_nav {
  background: #53297f !important;
}
/* navigation buttons */
.nav_button{
    font-family: 'Dosis', sans-serif;
    font-weight: 600;
    margin:.5vh
  }
/* Information about me */
.name{
    border-radius: 25px;
    background-color:#367880 ;
    padding: 3vh;
    padding-left: 10vh;
    margin: 3vh;
    text-align:left
  }
/* button spacing */
.btn{
  font-family: 'Dosis', sans-serif;
  font-weight: 600;
  padding: 1vh;
  margin-left: 4vh;
  margin-right: 4vh
}
/* welcome message */
.welcome{
  font-family: 'Playfair Display', serif;
  font-size: 3.5vh;
  margin-top: 2vh;
  margin-bottom: 2vh;
  margin-left: auto;
  margin-right: auto;
  background-color: rgb(212, 212, 212);
  color:rgb(0, 43, 35);
  border-radius: 10px;
  height: 15vh;
  width:27vw;
  padding: 2vh;
  text-align: center;
  
}
.button{
  margin-left: 1vh
}
/*flex boxes*/
.container {
  display: flex; /* create a flex container */
  /*have the div span the whole screen + change background color */
  position:fixed;
  width:100%;
  height:100%;
  /*changes all text to white*/
  color:rgb(212, 212, 212);
  background-color: rgb(12, 0, 22);
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