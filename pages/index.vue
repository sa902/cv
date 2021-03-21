<template language="markdown">
  <div class="">

     <!-- header -->
  <v-sheet class="fill-height" color="red lighten-2" elevation="0" height="350px" width="100%" >
    <v-container fill-height align="center" justify="center" >
      <v-row flat justify="center"  >

    <div class="">
      <p class="header-title">
        Sam Anderson
      </p>
      <p class="d-flex justify-center display-1">

        Developer
      </p>
    </div>

  </v-row>
  <v-row flat justify="center" >

    <v-col cols="3" class="d-flex justify-end " color="" >
      <v-list dark flat dense color="rgba(0,0,0,0)">
        <v-list-item> <v-list-item-icon><v-icon>mdi-home</v-icon></v-list-item-icon>55 Oaklands, Chippenham, Wiltshire </v-list-item>
        <v-list-item> <v-list-item-icon><v-icon>mdi-web</v-icon></v-list-item-icon>sa902.github.io </v-list-item>
      </v-list>
     </v-col>
     <v-col cols="3" class="d-flex justify-start"  color="" >


       <v-list dark flat dense color="rgba(0,0,0,0)">
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
      <p class="d-flex justify-center statement">
        I am a hardworking and dedicated individual with strong analytical skills and communication. Flexible and creative; a strong team player or can work individually on various tasks, performing them to a professional standard.
      </p>

      <div class="d-flex justify-center  sub-title ">
        <!-- <p class="sub-title"> -->
          Education
        <!-- </p> -->
      </div>
      <v-divider class="" width="100%" ></v-divider>
      <div class="d-flex justify-center">

        <v-card class="d-flex align-center justify-center" width="100%" dense flat tile >



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

      <v-list dense flat >
        <v-list-item v-for="skill in skills">
        <v-col cols="2" >

          <v-list-tile-title class="d-flex pr-5">
          {{skill.title}}
        </v-list-tile-title>
      </v-col>
      <v-col  >


          <v-sheet color="" elevation="0" height="100%" width="100%" class="pl-5">

            <v-progress-linear
            background-color="pink lighten-3"
            color="pink lighten-1"
            height="15"
            striped
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
     <v-col cols="7" >
       <div class="d-flex justify-center sub-title ">
         Work History

       </div>
       <div class="">
         <v-timeline>
           <v-timeline-item  v-for="job in jobs" small :color="job.color" fill-dot class="statement">
             <v-card elevation="4" color="" >
               <v-card-title class="d-flex justify-center pa-0 ma-0" >
                 {{job.title}} &nbsp
                 <div v-if="job.company" class="">
                  |  &nbsp  {{job.company}}
                 </div>
                  </v-card-title>
                  <v-card-subtitle class="d-flex justify-center pa-0 ma-0" >
                   {{job.date}}
                   </v-card-subtitle>
                   <!-- <v-list dense flat class="pa-0 ma-0">
                     <v-list-item tile dense flat v-for="item in job.items">
                       {{item}}
                      </v-list-item>
                    </v-list> -->
                    <div v-for="item in job.items" >
                      {{ item }}
                    </div>

                    {{job.desc}}
             </v-card>
            </v-timeline-item>
         </v-timeline>


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
    skills: [
      {
        title:"VueJS",
        level:15
      },
      {
        title:"java",
        level:20
      },
      {
        title:"html",
        level:20
      },
      {
        title:"python",
        level:50
      }
    ],
    jobs : [
      {
        title:"Teacher",
        company:"SISA Amata school",
        date:"1/08/2019-23/3/2020",
        color:"purple",
        desc:"Taught Maths,Science and English"

      },
      {
        title:"Software Dev",
        company:"SquidCard",
        date:"1/4/2019-1/7/2019",
        color:"red",
        desc:"Java EE / Spring Boot / Docker /  Payara Web server",



      },
      {
        title:"Freelance Dev",
        company:"",
        date: "25/11/2018 – 1/3/2019",
        color:"purple",
        desc:"Designing cashierless shopping using motion tracking and pose estimation. Matlab/Python/Tensorflow!"

      },
      {
        title:"Software Dev",
        company:"Moogsoft",
        date:"04/12/2017–31/10/2018",
        color:"red",
        desc:"Java EE, RabbitMQ, Tomcat, ES6 Docker ",

      },

    ]

  }),
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@600&display=swap');
.header-title{
  font-family: 'Work Sans', sans-serif;
  font-size: 85px;
  border-style: solid;
}
.sub-title{
  font-family: 'Work Sans', sans-serif;
  font-size: 25px;
}
.statement{
  font-size: 10px;
}
</style>
