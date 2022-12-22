<template>
  <div class="home">
    <div class="flex-container">
    
    <div class="item1">

      <div class="draw">
        /*drawing will go here*/
      </div>

      <div class="welcomeMessage">
        <p>Welcome to my corner of the internet</p>
      </div> 

      <div class="Linkbtn">
        <div class="q-pa-md q-gutter-sm">
          <!-- LinkedIn Button -->
          <q-btn class="button" href="https://www.linkedin.com/in/melbeshb/" color="brown-5" style="width:20%;font-size: 2em;font-weight: 600" label="Img" />
          <q-btn class="button" href="https://www.linkedin.com/in/melbeshb/" style="font-weight: 600; background: #D8815C; color: white; width:75%; font-size: 2em;" label="LinkedIn"/>

          <!-- GitHub -->
          <q-btn class="button" href="https://github.com/maryam-elbeshbishy" color="brown-5" style="width:20%;font-size: 2em;font-weight: 600" label="Img" />
          <q-btn class="button" href="https://github.com/maryam-elbeshbishy" style="font-weight: 600; background: #D8815C; color: white; width:75%; font-size: 2em;" label="GitHub" />

          <!-- Email -->
          <q-btn class="button" href="mailto: maryam.elbeshbishy@ryerson.ca" color="brown-5" style="width:20%;font-size: 2em;font-weight: 600" label="Img" />
          <q-btn class="button" href="mailto: maryam.elbeshbishy@ryerson.ca" style="font-weight: 600; background: #D8815C; color: white; width:75%; font-size: 2em;" label="Email" />

          <!-- Resume -->
          <q-btn class="button" href="" color="brown-5" style="width:20%;font-size: 2em;font-weight: 600" label="Img" />
          <q-btn class="button" href="" style="font-weight: 600; background: #D8815C; color: white; width:75%; font-size: 2em;" label="Resume" />
        </div>
        
      </div>
    </div>
    <div class="item2">
      <div class="q-pa-md q-gutter-sm">
          <q-btn class="button" style="font-weight: 600; background: #683227; color: white; width:24%; font-size: 1.8em;" label="About Me" to="/about"/>
          <q-btn class="button" style="font-weight: 600; background: #683227; color: white; width:24%; font-size: 1.8em;" label="Projects" to="/projects"/>
          <q-btn class="button" style="font-weight: 600; background: #683227; color: white; width:24%; font-size: 1.8em;" label="Art Portfolio" to="/art"/>
          <q-btn class="button" style="font-weight: 600; background: #683227; color: white; width:24%; font-size: 1.8em;" label="DevLogs" to="/devlogs"/>
      </div>

      <div class="Name">
        <p style="font-family:'Playfair Display';color: #683227; font-size:5em ">Maryam Elbeshbishy</p>
        <p style="font-weight:600; font-family:'Dosis', sans-serif; color: #683227;font-size:3em ">Computer Science</p>
        <p style="font-weight:600; font-family:'Dosis', sans-serif; color: #683227;font-size:3em">Toronto Metropolitan University</p>
      </div>

      <div class="Drawing2">
        <p>/*drawing2 will go here*/</p>
      </div>
    </div>

  </div>
    
    
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Dosis:wght@400;600;800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Dosis&family=Playfair+Display:wght@600&display=swap');
  .button{
    font-family: 'Dosis', sans-serif;
    font-weight: 600;
  }

  .Name{
    border-radius: 25px;
    background-color:#D8815C ;
    padding: 1em;
    padding-left: 5em;
    text-align:left

  }
  .flex-container {

    display: flex;
    
    justify-content: center; 
    align-items: stretch; 
    /* flex-flow: row wrap; */ 
    flex-direction: row; 
    flex-wrap: wrap; 
    align-content: stretch;

    background-color: #EBC9A4;
    height: 100%;
    padding: 3em;
    gap: 5px;

  }

  .flex-container > div{

    border-radius: 5px;
    padding: 3em;
  }


  .item1 { 
    /* flex:1 1 auto; */
    flex: 2 1 0;
  
  }
			
  .item2 { 
    /* flex:3 1 auto; */
    flex: 4 1 0;
    
  }
</style>
