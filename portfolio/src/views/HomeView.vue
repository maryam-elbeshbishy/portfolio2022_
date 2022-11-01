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
          <q-btn href="https://www.linkedin.com/in/melbeshb/" color="brown-5" label="Img" />
          <q-btn href="https://www.linkedin.com/in/melbeshb/" style="background: #D8815C; color: white" label="LinkedIn" />
        </div>

        <div class="q-pa-md q-gutter-sm">
          <q-btn href="https://github.com/maryam-elbeshbishy" color="brown-5" label="Img" />
          <q-btn href="https://github.com/maryam-elbeshbishy" style="background: #D8815C; color: white" label="GitHub" />
        </div>

        <div class="q-pa-md q-gutter-sm">
          <q-btn color="brown-5" label="Img" />
          <q-btn style="background: #D8815C; color: white" label="Resume" />
        </div>
      
        <div class="q-pa-md q-gutter-sm">
          <q-btn href="mailto: maryam.elbeshbishy@ryerson.ca" color="brown-5" label="Img" />
          <q-btn href="mailto: maryam.elbeshbishy@ryerson.ca" style="background: #D8815C; color: white" label="Email" />
        </div>
        
      </div>
    </div>
    <div class="item2">
      <div class="q-pa-md q-gutter-sm">
          <q-btn color="brown-5" label="About Me" to="/about"/>
          <q-btn color="brown-5" label="Projects" to="/projects"/>
          <q-btn color="brown-5" label="Art Portfolio" to="/art"/>
          <q-btn color="brown-5" label="DevLogs" to="/devlogs"/>
      </div>

      <div class="Name">
        <h1>Maryam Elbeshbishy</h1>
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
  q-btn{
    font-size: 7rem;
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
    padding: 15px;
    gap: 5px;

  }

  .flex-container > div{

    border-radius: 5px;
    padding: 50px;
  }


  .item1 { 
    /* flex:1 1 auto; */
    flex: 2 1 0;
  
  }
			
  .item2 { 
    /* flex:3 1 auto; */
    flex: 5 1 0;
    
  }
</style>
