<template>
  <div class="container-5">
    <div class="item-3">
      <div>
        <img src="..\img\TL.jpg" style="width:20vw; border-radius: 10px;display: block;margin-left: auto; margin-right: auto;margin-top:3vh; margin-bottom:3vh" alt="ART NOT LOADED">
      </div>
      <div class="title_side" style="color:rgb(0, 22, 2) ">
        Dev Logs
      </div>
      <div>
        <div>
          <q-btn class="btn" color="button_nav-4" text-color="white" style="font-weight: 600; width: 80%; font-size: 1.8em; margin-top: 2vh;" label="Home" to="/"/>
        </div>
        <div>
          <q-btn class="btn" color="button_nav-4" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="Art Portfolio" to="/art"/>
        </div>
        <div>
        <q-btn class="btn" color="button_nav-4" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="About Me" to="/about"/>
        </div>
        <div>
          <q-btn class="btn" color="button_nav-4" text-color="white" style="font-weight: 600; width:80%; font-size: 1.8em;margin-top: 2vh" label="Projects" to="/projects"/>
        </div>
      </div>
    </div>

    <div class="item-4">
      <div class="under_construction">
        <h2>Under Construction!<br> Come back soon :)</h2>
      </div>
      <!-- <div class="item" v-for="item in items" :key="item.id" style="color:black">
        <q-card class="my-card">
            <img src="https://cdn.quasar.dev/img/mountains.jpg">

            <q-card-section>
              <div class="text-h6">{{item.title}}</div>
              <div class="text-subtitle2">{{item.date}}</div>
              <div class="text-subtitle2">{{item.tools}}</div>

            </q-card-section>

            <q-card-section class="q-pt-none">
              {{item.description}}
            </q-card-section>
          </q-card>
      </div> -->
    </div>
  </div>
  </template>


<script>
import devItems from '../databases/devLogs.json'
export default {
    name: 'ProjectsPage',
    data() {
        return {
            items: devItems,
        }
    }
}
</script>

<style>
.bg-button_nav-4 {
  background: #06430c !important;
}
.container-5 {
  display: flex;

  /*changes all text to white*/
  color:rgb(212, 212, 212);
  background-color: rgb(0, 22, 2);
}

.under_construction{
  font-family: 'Playfair Display', serif;
  font-size: 6vh;
  margin-top: 15vh;
  margin-bottom: 2vh;
  margin-left: auto;
  margin-right: auto;
  background-color: rgb(212, 212, 212);
  color:rgb(6, 43, 0);
  border-radius: 10px;
  width: 80%;
  padding: 2vh;
  text-align: center;
}
</style>