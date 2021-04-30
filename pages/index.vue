<template language="markdown">
  <div class="">

     <!-- header -->
  <v-sheet class="fill-height ma-0 pa-0" color="#457B9D" elevation="0" height="280px" width="100%" >
    <v-container fill-height align="center" justify="center" >
      <v-row flat justify="center"  >

    <div class="header-title ma-0 pa-0">
      <!-- <p class=""> -->
        Sam Anderson
      <!-- </p> -->

    </div>

  </v-row>
  <v-row flat justify="center" >

    <v-col class="d-flex justify-center " color="" >
      <v-list dark flat dense color="rgba(0,0,0,0)">
        <v-list-item color=""> <v-list-item-icon><v-icon color="">mdi-home</v-icon></v-list-item-icon>55 Oaklands, Chippenham, Wiltshire </v-list-item>
        <v-list-item> <v-list-item-icon><v-icon>mdi-phone</v-icon></v-list-item-icon>07385242082 </v-list-item>
        <v-list-item> <v-list-item-icon><v-icon>mdi-email</v-icon></v-list-item-icon>samanderson902@gmail.com </v-list-item>
      </v-list>
     </v-col>

</v-row>
  </v-container>
  </v-sheet>
 <!-- header -->

<v-container fill-height>
  <v-row  >
    <v-col cols="5" >

      <div class="d-flex justify-center  ">
        <p class="sub-title">
          Personal Statement
        </p>
      </div>
      <v-divider></v-divider>
      <p class="d-flex justify-center statement pl-5">
      {{this.pstate}}
      </p>

      <div class="d-flex justify-center  sub-title ">
        <!-- <p class="sub-title"> -->
          Education
        <!-- </p> -->
      </div>
      <v-divider class="" width="100%" ></v-divider>
      <div class="d-flex justify-center">

        <v-card color="#F1FAEE" class="d-flex align-center justify-center" width="100%" dense flat tile >



            <v-list-item three-line>
              <img src="~/assets/charcoal.png" height="60px"alt="">
              <v-list-item-content>
                <v-list-item-title class="title pl-8">
                  Computer Science
                </v-list-item-title>
                <div class="overline pl-8">
                  BSc (Hons) 2:1
                </div>
                <v-list-item-subtitle class="pl-8">Focusing on Computer Vision, AI and ML</v-list-item-subtitle>
              </v-list-item-content>


            </v-list-item>
        </v-card>

      </div>
      <div class="d-flex justify-center  sub-title ">
        <!-- <p class="sub-title"> -->
          Skills
        <!-- </p> -->
      </div>
      <v-divider></v-divider>

      <v-list dense flat color="#F1FAEE" class="">
        <v-list-item v-for="skill in skills" class="pb-3">
        <v-col color="#F1FAEE" cols="3" >

          <v-list-tile-title class="d-flex pr-5">
          {{skill.title}}
        </v-list-tile-title>
      </v-col>

      <v-col  >


          <v-sheet color="#F1FAEE" elevation="0" height="100%" width="100%" class="pl-5">

            <v-progress-linear
            background-color="#457B9D"
            color="#1d3557"
            height="15"

            :value="skill.level"
            ></v-progress-linear>
           </v-sheet>
         </v-col>
        </v-list-item>


      </v-list>
     </v-col>
     <v-divider

       vertical
     ></v-divider>
     <!-- second column  -->
     <v-col cols="7"  >
       <div class="d-flex justify-center sub-title ">
         Work History

       </div>
       <v-divider></v-divider>
       <div class="">
         <div v-for="job in jobs" :key="job.id" class="pb-3">

         <!-- <v-timeline left > -->
           <!-- <v-timeline-item right  v-for="job in jobs" small :color="job.color" fill-dot class="statement"> -->
             <v-card  color="#F1FAEE" dense flat tile class="pa-0 ma-0">
               <v-card-title class="d-flex justify-center pa-0 ma-0 wh-title" >
                 {{job.title}} &nbsp
                 <div v-if="job.company" class="">
                  |  &nbsp  {{job.company}}
                 </div>
                  </v-card-title>
                  <v-card-subtitle class="d-flex justify-center pa-0 ma-0" >
                   {{job.date}}
                   </v-card-subtitle>
                   <div v-for="item in job.items" class="pt-1 statement">
                     <v-icon>mdi-chevron-right</v-icon>{{ item }}
                   </div>

                   <!-- <v-list dense flat class="pa-0 ma-0">
                     <v-list-item tile dense flat v-for="item in job.items">
                       <v-list-item-icon><v-icon>mdi-chevron-right</v-icon></v-list-item-icon>
                       {{item}}
                      </v-list-item>
                    </v-list> -->
                    <!-- <div v-for="item in job.items" >
                      {{ item }}
                    </div> -->


             </v-card>

            <!-- </v-timeline-item> -->
         <!-- </v-timeline> -->


     </div>
   </div>
      </v-col>
   </v-row>
</v-container>
</div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  data : () => ({
    pstate: ` I am a hardworking and dedicated individual with strong analytical skills and communication. Flexible and creative;
    a strong team player or can work individually on various tasks, performing them to a professional standard.
    `,
    skills: [
      {
        title:"Java",
        level:80
      },
      {
        title:"Python",
        level:80
      },
      {
        title:"Git",
        level:80
      },
      {
        title:"Vue JS",
        level:80
      },
      {
        title:"SQL",
        level: 70
      },

      {
        title:"Vuex",
        level:65
      },
      {
        title:"GraphQL",
        level: 55
      },
      {
        title:"NodeJS",
        level:50
      },
      {
        title:"Docker",
        level:40
      },

    ],
    jobs : [
      {
        title:"Owner - Lead tutor",
        company:"Apollo Tutoring",
        date:"19/07/2020-Present",
        color:"purple",
        desc:"",
        items:[
          "Created a Tutoring company for children and adults to deliver 1-to-1 programming lessons in a range of languages",
          "Created a website, log in portal and learning dashboard for students using Vue,Vuex, and NodeJS",
          "Manage an online presence and deliver effective marketing",

        // "Plan and deliver effective 1-to-1 programming lessons in a range of languages",
        // "Plan and deliver effective 1-to-1 computer science lessons"


        ],
        id:0
      },
      {
        title:"Lead English Teacher",
        company:"SISA Amata school",
        date:"1/08/2019-23/3/2020",
        color:"purple",
        desc:"",
        items:[
          "Produce engaging content in Maths,Science and English for students who did not speak English",
          "Created a Robotic and computer programming course for children",
          "Planned, Organised and managed lessons for children who needed extra English classes",
          "Tutored and mentored students on a 1-to-1 basis to increase English and Mathematical ability",

        ],
        id:1
      },
      {
        title:"Software Developer",
        company:"SquidCard",
        date:"1/4/2019-1/7/2019",
        color:"red",
        desc:"",
        items:[
          "Back end / Architecture role.",
"Java EE / Spring Boot / Docker /  Payara Web server",
"Redesigned  installer to use docker.",
"Created a new front end and updated existing backend to fit user requirements.",
"Led a team to create a voting system using microservice design pattern.",
],
        id:2
      },
      {
        title:"Freelance Developer",
        company:"",
        date: "25/11/2018 – 1/3/2019",
        color:"purple",
        desc:"",
        items:[
          "Designed and implemented a cashierless checkout system using object tracking, pose estimation and field detection",
          "Optimised a sports betting system using Python and Matlab",
          "Implemented a stripe checkout system for an ecommerce website"

        ],
        id:3
      },
      {
        title:"Software Developer",
        company:"Moogsoft",
        date:"04/12/2017–30/10/2018",
        color:"red",
        desc:"",
        items:[
          "JAva 8, JS ES6, JUnit, Powermock, Mockito, Git, Docker",
          "Worked in the integrations team providing custom API's allowing bidirectional communication between multiple products",
          "liaised  with the AI department to realise conceptual AI designs",
          "Worked closely with customers to implement bespoke solutions"
        ],
        id:4
      },

    ]

  }),

}
</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@600&display=swap');
.chgcol{
  background:  '#F1FAEE'
}
.header-title{
  font-family: 'Work Sans', sans-serif;

  font-size: 85px;
  /* border-style: solid; */
}
.sub-title{
  font-family: 'Work Sans', sans-serif;
  font-size: 25px;
}
.wh-title{
  font-family: 'Work Sans', sans-serif;
  font-size: 20px;
}
.statement{
  font-size: 15px;
}
</style>
