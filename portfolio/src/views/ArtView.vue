<template>
  <body style="overflow: hidden; height: 100vh;">
  <div class="container-4">

    <div class="item-3">
      <div>
        <img src="..\img\TL.jpg" style="width:20vw; border-radius: 10px;display: block;margin-left: auto; margin-right: auto;margin-top:3vh; margin-bottom:3vh" alt="ART NOT LOADED">
      </div>
      <div class="title_side">
        Art Portfolio
      </div>
      <div>
        <div>
          <q-btn class="btn" color="button_nav-2" text-color="white" style="font-weight: 600; width: 80%; font-size: 1.8em; margin-top: 2vh;" label="Home" to="/"/>
        </div>
        <div>
          <q-btn class="btn" color="button_nav-2" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="Projects" to="/projects"/>
        </div>
        <div>
        <q-btn class="btn" color="button_nav-2" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="About Me" to="/about"/>
        </div>
        <div>
          <q-btn class="btn" color="button_nav-2" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="DevLogs" to="/devlogs"/>
        </div>
      </div>
    </div>

    <div class="item-4">
      <div class="item" v-for="item in items" :key="item.id" style="color:black">
        <q-card class="my-card">
            <img src="https://cdn.quasar.dev/img/mountains.jpg">

            <q-card-section>
              <div class="text-h6">{{item.title}}</div>
              <div class="text-subtitle2">{{item.tools}}</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
              {{item.description}}
            </q-card-section>
          </q-card>
      </div>
    </div>

  </div>

</body>

  </template>


<script>
import artItems from '../databases/art.json'
export default {
    name: 'ProjectsPage',
    data() {
        return {
            items: artItems,
        }
    }
}
</script>

<style>

.bg-button_icon-1 {
  background: #56131a !important;
}
.bg-button_nav-2 {
  background: #8b5314 !important;
}
.container-4 {
  display: flex; /* create a flex container */
  /*have the div span the whole screen + change background color */
  /*changes all text to white*/
  height:100%;
  color:rgb(212, 212, 212);
  background-color: rgb(33, 24, 2);
}
.item-3 {
  flex:1;
  margin: 2vw;
  
}
.item-4 {
  flex: 4;
  overflow-y: auto;
}
.item {
    vertical-align: top;
    display: inline-block;
    text-align: center;
    width:43%;
}
.title_side{
  font-family: 'Playfair Display', serif;
  font-size: 6vh;
  margin-top: 2vh;
  margin-bottom: 2vh;
  margin-left: auto;
  margin-right: auto;
  background-color: rgb(212, 212, 212);
  color:rgb(43, 22, 0);
  border-radius: 10px;
  height: 15vh;
  width:20vw;
  padding: 2vh;
  text-align: center;
  
}
</style>