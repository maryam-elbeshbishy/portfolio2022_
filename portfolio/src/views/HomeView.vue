<!-- COLOR NEEDS TO BE CONFIGURED -->
<template>
  <div class="row bg-background_color" style="height:100vh">
    <div class="columns col-3"> 
      <div class="q-mr-md q-ml-md q-mt-sm">
        <q-img src="..\img\top_left_home.jpg"
        spinner-color="white"
        style="border-radius: 10px;" alt="ART NOT LOADED"/>
      </div>
        
      <div class="q-ma-md text-center">
        <q-card-section class="welcome_message bg-welcome_message text-welcome_message">
          <div class="text-h4">Welcome to my corner of the internet!</div>
        </q-card-section>
      </div>

      <div class="link_btn text-center">
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn text-link_btn"  style="width:90%;" href="https://www.linkedin.com/in/melbeshb/" label="LinkedIn" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn text-link_btn"  style="width:90%;" href="https://github.com/maryam-elbeshbishy" label="GitHub" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn text-link_btn"  style="width:90%;" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Email" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn text-link_btn"  style="width:90%;" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Resume" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn text-link_btn"  style="width:90%;" href="https://www.instagram.com/marilambb_draws/" label="Art Insta" /> 
      </div>
  </div>

  <div class="columns col-8"> 
    <div class="nav_btn text-center">
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn text-nav_btn"  style="width:23%;" label="About Me" to="/about"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn text-nav_btn"  style="width:23%;" label="Tech Portfolio" to="/projects"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn text-nav_btn"  style="width:23%;" label="Art Portfolio" to="/art"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn text-nav_btn"  style="width:23%;" label="Dev Logs" to="/devlogs"/> 
    </div>

    <div>
      <q-card-section class="q-ma-lg bg-about_message text-about_message" style="border-radius: 10px">
          <div class="text-h3 q-ma-lg" style="font-family:'Playfair Display';">Maryam Elbeshbishy</div>
          <div class="text-h4 q-ma-lg" style="font-family:'Dosis';">Computer Science - Toronto Metropolitan University</div>
          <div class="text-h5 q-ma-lg" style="font-family:'Dosis';">Hi! As you may have seen my name is Maryam, Im currently working as a Research Assistant
        at Ryerson University, I am quite passionate about Data Science and XR Development, currently taking courses in both to expand my knowledge! Check the rest of my website for more
      information. <br> PS. Any art on this website was created by me!</div>
      </q-card-section>
    </div>

    <div class="q-ma-lg">
        <q-img src="..\img\bottom_right_home.jpg"
        spinner-color="white"
        style="border-radius: 10px;" alt="ART NOT LOADED"/>
      </div>
    
  </div>
</div>

</template>

<script>

</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Dosis:wght@400;600;800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Dosis&family=Playfair+Display:wght@600&display=swap');

/* background color */
.bg-background_color{
  background:#051301 !important;
}
/* column styling */
.columns{
  margin: 2vw;
}
/* welcome message */
.welcome_message{
  font-family: Playfair-Display;
  border-radius: 10px;
}
.bg-welcome_message{
  background: rgb(0, 43, 35) !important; 
}
.text-welcome_message{
  color: #f1e2ff !important;
}

/* link buttons */
.link_btn{
  font-family: Dosis;
  font-weight: 600;
}
.bg-link_btn{
  background: #ad5641 !important
}
.text-link_btn{
  color: #fff1ee !important
}

/* nav buttons */
.nav_btn{
  font-family: Dosis;
  font-weight: 600;
}
.bg-nav_btn{
  background: #2fa212 !important
}
.text-nav_btn{
  color: #daf0d0 !important
}
/* About Me Blurb */
.bg-about_message{
  background: rgb(113, 14, 109) !important; 
}
.text-about_message{
  color: #f1e2ff !important;
}
</style>