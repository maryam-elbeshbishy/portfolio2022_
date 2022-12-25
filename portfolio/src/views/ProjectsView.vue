<template>
  <body style="overflow: hidden; height: 100vh;">
  <div class="container-2">

    <div class="item-3">
      <div>
        <img src="..\img\proj.jpg" style="width:20vw; border-radius: 10px;display: block;margin-left: auto; margin-right: auto;margin-top:3vh; margin-bottom:3vh" alt="ART NOT LOADED">
      </div>
      <div class="title_side" style="color:rgb(0, 27, 41) ">
        Projects
      </div>
      <div>
        <div>
          <q-btn class="btn" color="button_nav-3" text-color="white" style="font-weight: 600; width: 80%; font-size: 1.8em; margin-top: 2vh;" label="Home" to="/"/>
        </div>
        <div>
          <q-btn class="btn" color="button_nav-3" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="Art Portfolio" to="/art"/>
        </div>
        <div>
        <q-btn class="btn" color="button_nav-3" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="About Me" to="/about"/>
        </div>
        <div>
          <q-btn class="btn" color="button_nav-3" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="DevLogs" to="/devlogs"/>
        </div>
      </div>
    </div>

    <div class="item-4">
      <div class="item-p" v-for="item in items" :key="item.id" style="color:rgb(0, 27, 41)">
        <q-card class="my-card" style="font-family:'Dosis'">
            <img :src="require(`../img/proj/${item.image}`)" style="width:20vw; border-radius: 10px;display: block;margin-left: auto; margin-right: auto">
            <q-card-section style="background: #b4d9e9">
              <div class="text-h5"><b>{{item.title}}</b></div>
              <div class="text-h6">{{item.tools}}</div>
              <div class="text-h6">{{item.date}}</div>
              

            </q-card-section>

            <q-card-section class="q-pt-none" style="background: #b4d9e9">
                {{item.description}}
            </q-card-section>
          </q-card>
      </div>
    </div>

  </div>

</body>

  </template>


<script>
import projItems from '../databases/projects.json'
export default {
    name: 'ProjectsPage',
    methods: {

    },
    data() {
        return {
            items: projItems,
          
        }
    }
}
</script>

<style>
.bg-button_nav-3 {
  background: #1b6686  !important;
}
.container-2 {
  display: flex; /* create a flex container */
  /*have the div span the whole screen + change background color */
  /*changes all text to white*/
  height:100%;
  color:rgb(212, 212, 212);
  background-color: rgb(0, 27, 41);
}
.item-3 {
  flex:1;
  margin: 2vw;
  height:100vh
  
}
.item-4 {
  flex: 4;
  overflow-y: auto;
}
.item-p {
    vertical-align: top;
    display: inline-block;
    text-align: center;
    width:43%;
    margin: 4vh;
}
</style>