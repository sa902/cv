<template lang="html">
  <div class="">

    <v-sheet class="fill-height ma-0 pa-0" color="#457B9D" elevation="0" height="270px" width="100%" >
      <v-container fill-height align="center" justify="center" >
        <v-row flat justify="center"  >

          <div class="header-title">

              Sam Anderson


          </div>

        </v-row>
        <v-row flat dense justify="center" >

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

    <v-card  dense flat tile color="rgba(0,0,0,0)" height="500px" width="85%">

      <v-card-text class="px-10 black--text">
        <h3>
        Dear Sir/Madam,
      </h3>
      <br>
        This letter is to express my interest in your Front End developer Role.
        With a bachelors in Computer Science, my hands on experience as a backend engineer and
        my experience as a classroom teacher/private tutor I believe I will be a great fit for your company.

        <br> <br>
        <p>
        During my time in Thailand I worked as a teacher and most recently I started a programming school for children aged 8-18. Over the past 6 months I have taught over 20 students python, java and on occasion Godot.
      </p>
      <p>
        I saw lockdown as a perfect time to use the skills I had most recently used (teaching) and learn something new that had always interested me, front end development. Having worked as a backend developer (using Java) and as a freelance developer (an AI MVP using Python) I want to shift into working in the front end.
        I played with a few different tech stacks and settled on Vue (Nuxt eventually), Vuetify, NodeJS (for my endpoints) and GraphQL. I have really enjoyed using these modern frameworks as they are friendly to developers and well documented.
        <br> I am looking for an opportunity that will help me build upon these skills in a friendly environment that values education. This is what makes me want to work for you so much.
      </p>

      <p>
        My teaching style is a blend between eastern thought and western sensibilities.
        It is a blend between the easts concept of "come and figure it out for yourself" and the wests approach to guided study.
        I give students the tools to solve the problem but then the freedom to explore their own solutions. It's only after they have their own solution can we talk about other possibilities.
        I treat coding and by extension computer science as an art form. That's really the beauty of coding and what makes it so fun to teach, the possibilities are nearly endless.
        I find students tend to enjoy this style and as well as myself. For this reason, I enjoy doing and receiving code reviews.
      <br>  My attitude towards programming is the same as my teaching style. I enjoy being given a challenge and the opportunity to learn myself as well as being in an environment that will not shun someone for asking questions if they need help.
      </p>

<p>
        I have looked at your website and your products.
        I am blown away by how accessible labsims has made chemistry and bioscience learning. I am jealous of those who get to use it and would love to have a play with it myself. During this pandemic I would enjoy learning a bit more about the coronaviruses and how vaccinations work!
        <br> The smart worksheet software you offer looks really good for teachers and students. Again, I wish this was used at my university when I was studying. From my perspective as a teacher, even though I taught younger children, thinking of and writing questions was time consuming as well as challenging. Having it all automated will make life so much easier.

      <br>  It reminds me of a project my friends and I tried to create while at university. We noticed that often exam papers would follow a similar  structure and often contain similar questions. To avoid complex revision we tried to build a piece of software that would learn these patterns and predict a number of exam questions in increasing likelihood.

        Unfortunately, like most AI projects, we lacked sufficient data to train our models properly. We only had access to 2 past papers.
      </p>






        Your company and your mission excites me. I have a passion for education and believe that humans have an uncapped ability to learn anything. I feel as if I would really fit in well in your company.

        Regards,
        Sam


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
        title:"Back End experience",
        content:
        `I have worked professionally as a backend engineer using Java (And when required JS) and use Node.js for personal passion projects.
        I've taken a liking to Strapi, it handles all my APIs and data base for me as well as providing an easy to use login portal for customers.

        `
      },
      {
        title:"EdTech experience",
        content: `
        During lockdown I have been working as programming tutor. This has given me experience in a teaching environment and an
        understanding of the pupil's perspective.
        `
      },

      {
        title:"Vue",
        content:
        `Vue has been my main language during the lockdown period.
        I have made a couple of interesting projects lockdown. One is a site for a magazine aimed at artists in the Liverpool area
        The other is my own programming with a learning environment that hosts lesson files, quizzes and tracks a student's learning progress.
        Additionally, this CV is written in Vue!
        `

},


//
//       {
//         title:"API Usage",
//         content:`REST is ubiquitous on the web and I have most recently used it with Firebase and Strapi.
//         I have used SOAP and STOMP to consume data from Network Rail. This was a project to calculate liklihood of a delayed train
//         and ability to claim a refund!
//         `
//       },
      {
        title:"SQL and NoSQL",
        content:"At Squidcard and Moogsoft I used SQL databases. For my own projects and I use google firebase or Strapi with GraphQL. "
      },

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
