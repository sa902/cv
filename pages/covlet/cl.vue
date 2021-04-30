<template lang="html">
  <div class="">

    <v-sheet class="fill-height ma-0 pa-0" color="#457B9D" elevation="0" height="280px" width="100%" >
      <v-container fill-height align="center" justify="center" >
        <v-row flat justify="center"  >

          <div class="">
            <p class="header-title ma-0 pa-0">
              Sam Anderson
            </p>

          </div>

        </v-row>
        <v-row flat justify="center" >

          <v-col class="d-flex justify-center " color="" >
            <v-list dark flat dense color="rgba(0,0,0,0)">
              <v-list-item color=""> <v-list-item-icon><v-icon color="">mdi-home</v-icon></v-list-item-icon>55 Oaklands, Chippenham, Wiltshire </v-list-item>
              <!-- <v-list-item> <v-list-item-icon><v-icon>mdi-web</v-icon></v-list-item-icon>sa902.github.io </v-list-item> -->
              <v-list-item> <v-list-item-icon><v-icon>mdi-phone</v-icon></v-list-item-icon>07385242082 </v-list-item>
              <v-list-item> <v-list-item-icon><v-icon>mdi-email</v-icon></v-list-item-icon>samanderson902@gmail.com </v-list-item>
            </v-list>
          </v-col>
          <!-- <v-col  cols="2"class="d-flex justify-start"  color="" >


          <v-list dark flat dense color="rgba(0,0,0,0)">
        </v-list>
      </v-col> -->
    </v-row>
    <v-row justify="center" >

    <v-card  dense flat tile color="rgba(0,0,0,0)" height="500px" width="80%">

      <v-card-text class="px-10 black--text">
        <h3>
        Dear Sir/Madam,
      </h3>
      <br><br>
        This letter is to express my interest in your Associate Digital Tutor role.
        With a bachelors in Computer Science, my hands on experience as a backend engineer and
        my experience as a classroom tutor and private tutor
            I believe I will be an asset to your company.

        <br> <br>
I have a passion teaching and passing my knowledge on to the next generation of programmers.
I feel a great sense of pride in my students when they understand a new topic and complete a complex programming problem.
I believe that knowledge about tech should be open to all.
<br><br>
Your listed requirements match my background and skills. A few I would like to highlight are:
<v-list dense flat color="rgba(0,0,0,0)" class="pa-0 ma-0 text--black">


<v-list-item v-for="item in items"  class="pa-0 ma-0">
  <v-list-item-icon><v-icon>mdi-chevron-right</v-icon></v-list-item-icon>
   <v-list-item-content>
     <v-list-item-title>{{item.title}}</v-list-item-title>
     {{item.content}}
</v-list-item-content>
</v-list-item>


</v-list>
<br><br>
Below is a copy of my CV with my recent experience. Thank you for your consideration and I look forward to hearing back from you.

<br><br>
Sincerely,
<br>
<br>
<h3>
Sam Anderson
</h3>

      </v-card-text>
    </v-card>
  </v-row>
  </v-container>
</v-sheet>
  </div>
</template>

<script>
export default {
  data : () =>({
    items  : [
      {
        title:"Java",
        content:`This was the main language used in my past two developer roles. At Moogsoft we used Java 8 and Squidcard Java EE with springboot.
        Gradle was used at moogsoft and Maven at squidcard
        With a license, Intellij is my preffered IDE. In the meantime I settle for Atom.
        In terms of testing I have used JUnit, Mockito and PowerMock
         `
      },
      {
        title:"Python:",
        content:`
        Python was the first language I learned and I have used it for many years both
        professionally and personally.
        I have used it at my
        \n
        I regularly complete coding challenges on codewars and project eular.
        I also mainly tutor with python`
      },
//
//       {
//         title:"API Usage",
//         content:`REST is ubiquitous on the web and I have most recently used it with Firebase and Strapi.
//         I have used SOAP and STOMP to consume data from Network Rail. This was a project to calculate liklihood of a delayed train
//         and ability to claim a refund!
//         `
//       },
//       {
//         title:"SQL and NoSQL",
//         content:"At squidcard and moogsoft I used SQL databases. For my own projects and I use google firebase and GraphQL. "
//       },
//
// {
//   title:"Docker",
//   content:"While at SquidCard I re-designed the installer to provide a containerized solution."
// },
// {
//   title:"Git",
//   content:"I use git cli to manage my work and projects. I host a couple of sites on github pages!"
// },




    ]

  })
}
</script>

<style lang="css" scoped>
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
.boop{
  font-size: 15px;
  color:black;

}
</style>
