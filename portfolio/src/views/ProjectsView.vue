<template>
  <div class="container-2">
    <div class="item_div">
      <q-btn class="nav_button" color="button_icon-2" text-color="white" style="font-weight: 600; width:20%; font-size: 3.5em; margin-right: 25vh;font-family: 'Playfair Display', serif;" label="Projects"/>
      <q-btn class="nav_button" color="button_nav-2" text-color="nav_btn" style="font-weight: 600; width:15%; font-size: 1.8em;" label="Home" to="/"/>
      <q-btn class="nav_button" color="button_nav-2" text-color="nav_btn" style="font-weight: 600; width:15%; font-size: 1.8em;" label="Projects" to="/projects"/>
      <q-btn class="nav_button" color="button_nav-2" text-color="nav_btn" style="font-weight: 600; width:15%; font-size: 1.8em;" label="Art Portfolio" to="/art"/>
      <q-btn class="nav_button" color="button_nav-2" text-color="nav_btn" style="font-weight: 600; width:15%; font-size: 1.8em;" label="DevLogs" to="/devlogs"/>
    </div>

    <div class="item_div">
      <figure class="item" v-for="item in items" :key="item.id">
            

            <figcaption>
                <h3> 
                    <a :href="item.github">
                    <!-- <img class="link" src="../assets/Images/githubLogoBlack.png"> -->
                    </a>
                    <b>{{item.title}}</b>
                </h3>
                <h4>{{item.tools}}</h4>
                <p style="text-align: left;">
                {{item.description}}</p>

            </figcaption>
        </figure>
    </div>
  </div>
  </template>


<script>
import ProjectItems from '../databases/projects.json'
export default {
    name: 'ProjectsPage',
    data() {
        return {
            items: ProjectItems,
        }
    }
}
</script>

<style>
.text-nav_btn {
  color: #0a0b4d !important;
}
.bg-button_col-2 {
  background: #d57962 !important;
}
.bg-button_icon-2 {
  background:  #1d214b!important;
}
.bg-button_nav-2 {
  background: #9fafd5 !important;
}
.container-2 {
  display: flex;
  flex-direction: column;
  

  /*changes all text to white*/
  color:rgb(205, 213, 255);
  background-color: rgb(0, 3, 34);
}
.item_div{
  margin: 4vh;
}
.item {
    vertical-align: top;
    display: inline-block;
    text-align: center;
    width:29%
}
</style>