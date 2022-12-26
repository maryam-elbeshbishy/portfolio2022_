<template>
 <div class="row bg-bg_about" style="height:100vh">
    <div class="columns col-3"> 
      <div class="q-mr-md q-ml-md q-mt-sm q-mb-lg text-center">
        <q-img src="..\img\pfp.jpg"
        spinner-color="white"
        style="border-radius: 20px;width:70%;" alt="ART NOT LOADED"/>
      </div>

      <div class="link_btn text-center">
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn_about text-link_btn_about"  style="width:90%;" href="https://www.linkedin.com/in/melbeshb/" label="LinkedIn" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn_about text-link_btn_about"  style="width:90%;" href="https://github.com/maryam-elbeshbishy" label="GitHub" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn_about text-link_btn_about"  style="width:90%;" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Email" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn_about text-link_btn_about"  style="width:90%;" href="mailto: maryam.elbeshbishy@ryerson.ca" label="Resume" /> 
        <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-link_btn_about text-link_btn_about"  style="width:90%;" href="https://www.instagram.com/marilambb_draws/" label="Art Insta" /> 
      </div>
    </div>

    <div class="columns col-8">
      <div class="nav_btn text-center">
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_about text-nav_btn_about"  style="width:23%;" label="About Me" to="/about"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_about text-nav_btn_about"  style="width:23%;" label="Tech Portfolio" to="/projects"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_about text-nav_btn_about"  style="width:23%;" label="Art Portfolio" to="/art"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_about text-nav_btn_about"  style="width:23%;" label="Dev Logs" to="/devlogs"/> 
      </div>

    <div>
      <q-card-section class="q-ma-lg bg-about_me_message text-about_me_message" style="border-radius: 10px">
          <div class="text-h4 q-ma-lg" style="font-family:'Playfair Display';">A Little About Me...</div>
          <div class="text-h5 q-ml-lg q-mr-lg" style="font-family:'Dosis';"><b>Technology</b></div>
          <div class="text-h5 q-ml-lg q-mr-lg q-mb-md" style="font-family:'Dosis';">
            Currently, my biggest passion is learning about <b>virtual reality</b>, which the driving force in me taking the leap to 
            <b>learn unity and C# through</b> a course held by Circuit Stream, to learn how to <b>create XR experiences</b>, ranging from AR mobile 
            applications to creating a simple game in VR
            <br>
            Along with that, I am quite passionate about learning more technologies related to Data Science. After having learnt many libraries that 
            are useful in Python, I would like to learn technologies that deal with big data!</div>
          <div class="text-h5 q-ml-lg q-mr-lg" style="font-family:'Dosis';"><b>Hobbies</b></div>
          <div class="text-h5 q-ml-lg q-mr-lg q-mb-md" style="font-family:'Dosis';">
            Recently, I've picked up many hobbies that I feel fullfill my life and ultimately help regulate my attention span. These hobbies include <b>drawing</b>> (mainly 
            digital, using procreate), <b>reading, playing piano and solving rubicks cubes</b>! Playing piano would have to be my favorite hobby at the moment, since it has 
            been a life long dream, and after a few years of contemplating whether it was worth I've decided to self teach myself!  
            <br>
            Fun fact: My lowest time to solve a standard rubicks cube is ~41sec! 
          </div>
      </q-card-section>
    </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
/* Columns styling (margins etc.) from HomeView.vue*/
.bg-bg_about{
  background: #322243 !important;
}
/* link buttons colors (style inherited from HomeView.vue) */
.bg-link_btn_about{
  background: #ad4190 !important;
}
.text-link_btn_about{
  color: #fff1ee !important;
}

/* nav buttons */
.bg-nav_btn_about{
  background: #1240a2 !important;
}
.text-nav_btn_about{
  color: #daf0d0 !important;
}

/* About Me */
.bg-about_me_message{
  background: rgb(14, 113, 16) !important; 
}
.text-about_me_message{
  color: #f1e2ff !important;
}
</style>