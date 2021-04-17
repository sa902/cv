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
        This letter is to express my interest in your Frontend Developer role.
        With a bachelors in Computer Science, my hands on experience as a backend engineer and
        my recent experience developing JAMStack web apps using Vue.js, Vuex for statement management and node.js.
        With these skills I believe I will be an asset to your company.

        <br> <br>
I enjoy being challenged and working with projects that allow me to expand my knowledge and increase my skillset.
Having used Vue.JS to develop some projects over the lockdown period I would like to expand my knowledge in a professional environment.
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
        title:"HTML5, CSS3, SASS:",
        content:"The foundation of the web and the first stack of languages I learned. I started my developing career as the web transitioned from HTML4 to HTML 5. As such it is a staple in my arsenal."
},
{
  title:"Javascript ES6:",
  content:"This was the language I used to create integrations between Moogsoft AIOPS and external applications."
},
{
  title:"Docker",
  content:"While at SquidCard I re-designed the installer to provide a containerized solution."
},
{
  title:"Git",
  content:"I use git cli to manage my work and side projects."
},
{
  title:"Vuex:",
  content:"Vue has been my main language during the lockdown period. I have made a few interesting projects utilizing firebase for user auth on static sites, strapi (with GraphQL) for content management and providing API endpoints."
},
{
  title:"Vue.JS:",
  content:"To control login status of users!"
}


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
