<template>
  <div class="row bg-bg_project" style="height:100vh">
    <div class="columns col-3"> 
      <div class="q-mr-md q-ml-md q-mt-sm">
        <q-img src="..\img\proj.jpg"
        spinner-color="white"
        style="border-radius: 10px;" alt="ART NOT LOADED"/>
      </div>
        
      <div class="q-ma-md text-center">
        <q-card-section class="welcome_message bg-project_title text-project_title">
          <div class="text-h5"> Work Experience, Certificates <br> and Personal Projects </div>
        </q-card-section>
        <q-card-section class="q-mt-md info_message bg-project_message text-project_message">
          <div class="text-body1"> Here you can find all I've learned outside of class! Relevant work experience, followed by 
            certificates collected through completed courses and ending with personal projects!</div>
        </q-card-section>
      </div>

      <div class="link_btn text-center">
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_project text-nav_btn_project"  style="width:90%;" label="Home" to="/"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_project text-nav_btn_project"  style="width:90%;" label="About Me" to="/about"/>
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_project text-nav_btn_project"  style="width:90%;" label="Art Portfolio" to="/art"/> 
      <q-btn class="q-ma-sm button text-h5 text-weight-bold bg-nav_btn_project text-nav_btn_project"  style="width:90%;" label="Dev Logs" to="/devlogs"/> 
      </div>
    </div>

    <div class="columns col-8">
      <q-scroll-area 
        :thumb-style="thumbStyle"
        :bar-style="barStyle"
        :visible="true"
        style="height: 90vh; max-width: 97%;">
        <!-- Work Experience -->
        <div class="q-pa-sm q-mr-sm">
          <q-carousel
            v-model="proj_start"
            transition-prev="slide-right"
            transition-next="slide-left"
            swipeable
            animated
            control-color="white"
            navigation-icon="radio_button_unchecked"
            navigation
            padding
            arrows
            height="45vh"
            class="bg-work_exp text-white shadow-1 rounded-borders"
          >
            <q-carousel-slide  v-for="item in W_items" :key="item.id" :name="item.title" class="column no-wrap">

              <div class="q-mt-md text-h6 title">
                {{ item.title }}
              </div>
              <div class="q-mt-sm text-body1 items">
                {{ item.place }}
              </div>
              <div class="q-mt-sm text-subtitle2 items">
                {{ item.date }}
              </div>
              <div class="q-mt-sm text-body2 items">
                {{ item.description }}
              </div>
              <div class="q-mt-sm text-body2 items">
                <b>Tools Used -</b> {{ item.tools }}
              </div>
              <div class="q-mt-sm text-body2 items">
                <b>Skills Learnt -</b> {{ item.skills}}
              </div>
            </q-carousel-slide>
          </q-carousel>
        </div>

      <!-- Certificates -->
      <div class="q-pa-sm q-mr-sm">
          <q-carousel
            v-model="cert_start"
            transition-prev="slide-right"
            transition-next="slide-left"
            swipeable
            animated
            control-color="white"
            navigation-icon="radio_button_unchecked"
            navigation
            padding
            arrows
            height="45vh"
            class="bg-cert text-white shadow-1 rounded-borders"
          >
            <q-carousel-slide  v-for="item in C_items" :key="item.id" :name="item.title" class="row">
              <div class="col-5">
                <img :src="require(`../img/certs/${item.image}`)" class="certs_img" />
              </div>
              <div class="col-6 q-mt-md">
                <p class="text-h5 title">{{ item.title }}</p>
                <p class="text-body1 items"><b>Skills Learnt -</b>{{ item.skills }}</p>
              </div>
              
            </q-carousel-slide>
          </q-carousel>
        </div>

      <!-- Projects -->
      <div class="q-pa-md row items-start q-gutter-md text-proj_card_text" >
        <q-card v-for="item in P_items" :key="item.id" class="my-card proj_card">
          <img :src="require(`../img/proj/${item.image}`)" class="proj_img" >

          <q-card-section class="title bg-proj_card_title">
              <div class="text-h6 "><b>{{item.title}}</b></div>
              <div class="text-body2 items">{{item.tools}}</div>
              <div class="text-body2 items">{{item.date}}</div>
          </q-card-section>

          <q-card-section class="items bg-proj_card_desc">
            {{item.description}}title
          </q-card-section>
        </q-card>
      </div>

      </q-scroll-area>
    </div>
  </div>
</template>


<script>
import projItems from '../databases/projects.json'
import workItems from '../databases/workExp.json'
import certItems from '../databases/certs.json'
import { ref } from 'vue'
export default {
    name: 'ProjectsPage',
    methods: {

    },
    data() {
        return {
            proj_start: ref('Research Assisstant (Data Science)'),
            cert_start: ref('Data Quest Python Basics'),
            P_items: projItems,
            W_items: workItems,
            C_items: certItems,
            thumbStyle: {
              right: '4px',
              borderRadius: '5px',
              backgroundColor: '#ffffff',
              width: '5px',
              opacity: 0.75
            },

            barStyle: {
              right: '2px',
              borderRadius: '9px',
              backgroundColor: '#027be3',
              width: '9px',
              opacity: 0.2
            }
        }
    }
}
</script>

<style>
/* Columns styling (margins etc.) from HomeView.vue*/
.bg-bg_project{
  background: #223e43 !important;
}

/* nav buttons */
.bg-nav_btn_project{
  background: #a21231 !important;
}
.text-nav_btn_project{
  color: #daf0d0 !important;
}

/* Title Left hand */
.bg-project_title{
  background: rgb(101, 113, 14) !important; 
}
.text-project_title{
  color: #f1e2ff !important;
}

/* Message Left Hand */
.bg-project_message{
  background: rgb(47, 14, 113) !important; 
}
.text-project_message{
  color: #f1e2ff !important;
}
.info_message{
  font-family: Nunito;
  border-radius: 10px;
}

/* Work Experience background and text */
.bg-work_exp{
  background: rgb(30, 50, 47) !important; 
}
.text-work_exp{
  color: rgb(8, 154, 101) !important; 
}

/* work exp Styling */
.bg-work_exp{
  background: rgb(14, 14, 113) !important; 
}
.title{
  font-family: 'Playfair Display';
}
.items{
  font-family: 'Nunito';
}

/* Project Styling */
.proj_card{
  width: 30vw;
}
.proj_img{
  width:10vw !important;
  border-radius: 10px;
  display: block;
  margin-left: auto; 
  margin-right: auto
}
.bg-proj_card_title{
  background: rgb(110, 14, 113) !important; 
}
.bg-proj_card_desc{
  background: rgb(206, 126, 207) !important; 
}
.text-proj_card_text{
  color:#feffff
}

/* certificate styling */
.certs_img{
  width: 18vw !important;
}
.bg-cert{
  background: rgb(14, 113, 75) !important; 
}
</style>