<template>
  <div class="container-2">
    <div class="item">
      <q-btn class="nav_button" color="button_icon" text-color="white" style="font-weight: 600; width:25%; font-size: 2.5em; margin-right: 20vh;font-family: 'Playfair Display', serif;" label="Art Portfolio"/>
      <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:15%; font-size: 1.8em;" label="Home" to="/"/>
      <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:15%; font-size: 1.8em;" label="Projects" to="/projects"/>
      <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:15%; font-size: 1.8em;" label="About Me" to="/about"/>
      <q-btn class="nav_button" color="button_nav" text-color="white" style="font-weight: 600; width:15%; font-size: 1.8em;" label="DevLogs" to="/devlogs"/>
    </div>

    <div class="item">
      <figure class="item" v-for="item in items" :key="item.id">
            <!-- <img class="projImg" :src="require(../assets/ProjectsImg/${item.image})" alt="PROJECT IMAGE"/> -->

            <figcaption class="caption">
                <h2> 
                    <b>{{item.title}}</b>
                </h2>
                <h4>{{item.tools}}</h4>
                <p>
                {{item.description}}</p>

            </figcaption>
        </figure>
    </div>
  </div>
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
.container-5 {
  display: flex;
  flex-direction: column;
  

  /*changes all text to white*/
  color:rgb(212, 212, 212);
  background-color: rgb(22, 0, 8);
}
.item{
  margin: 4vh;
}
</style>