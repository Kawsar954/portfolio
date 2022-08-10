<template>
  <v-app id="inspire">
    <v-app-bar app elevation="0" dark>
      <v-subheader><h1 class="blue--text text--darken-1">Kawsar<span class="yellow--text">Ahmed</span></h1></v-subheader>
      <v-tabs center-active right background-color="transparent" active-class="active-tab">
        <v-tab>Home</v-tab>
        <v-tab>About</v-tab>
        <v-tab>Blog</v-tab>
        <v-tab>Contact</v-tab>
      </v-tabs>
      <v-btn large color="green" class="white--text ml-10">Send Email</v-btn>
    </v-app-bar>
    <v-main style="background-color: blanchedalmond;">
      <section class="intro-section" id="home">
        <v-row class="align-center px-10" style="height: 690px;">
          <v-col lg="6" cols="6" class="pa-6 font-weight-bold py-16">
            <h2 class="display-2">Software <span class="light-blue--text text--accent-2">Design</span> & <span class="pink--text text--darken-1">Developer</span></h2>
            <v-subheader>Hi, I am Kawsar, design and develop software.</v-subheader>
            <br>
            <v-btn medium elevation="5" color="green" class="white--text mt-10 px-10 py-5">Hire me</v-btn>
            <v-btn medium elevation="5" color="red" class="white--text mt-10 ml-10 px-10 py-5">Contact</v-btn>
            <v-row class="mt-16">
              <v-chip class="px-4 ma-3" color="primary">
                <v-icon left size="20">mdi-facebook</v-icon>
                facebook
              </v-chip>
              <v-chip class="px-4 ma-3" color="info">
                <v-icon left size="20">mdi-linkedin</v-icon>
                Linkdin
              </v-chip>
              <v-chip class="px-4 ma-3" color="dark">
                <v-icon left size="20">mdi-github</v-icon>
                Github
              </v-chip>
              <v-chip class="px-4 ma-3" color="#01ff56">
                <v-icon left size="20">mdi-whatsapp</v-icon>
                whatsapp
              </v-chip>
            </v-row>
          </v-col>
          <v-col>
            <v-img src="@/assets/images/kawsar.jpg" style="height: 600px; border-radius: 50%;"></v-img>
          </v-col>
        </v-row>
      </section>
      <section class="about-me" id="about">
        <v-img class="pa-10" height="500" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)" src="@/assets/images/Home-office.jpeg">
          <v-row justify="center" class="align-center">
            <v-col lg="6" cols="6">
              <v-card class="text-center pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                <v-card-subtitle class="green--text font-weight-bold">ABOUT MYSELF</v-card-subtitle>
                <h4 class="display-1 font-weight-regular">
                  My name is Kawsar Ahmed. I completed my B.Sc in CSE from World University of Bangladesh. I am a quick learner and hard working person. I like to doing coding problem.
                </h4>
                <v-btn large elevation="5" color="pink" class="white--text mt-10 px-10 py-5">Download Resume
                  <v-icon>mdi-download</v-icon>
                </v-btn>
              </v-card>
            </v-col>
            <v-col lg="6" cols="6">
              <v-card class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                <div class="py-1" v-for="(item,index) in items" :key="index">
                  <label>{{ item.title }}</label>
                    <v-progress-linear
                      :color="item.color"
                      height="15"
                      :value="item.value"
                      ></v-progress-linear>
                </div>
              </v-card>
            </v-col>
          </v-row>
        </v-img>
      </section>
      <section class="educaion py-6">
                <v-container>
                    <h4 class="display-2 text-center">Education</h4>
                    <v-row class="py-8">
                        <v-col cols="12" lg="6">
                            <v-card class="pa-6 rounded-xl " elevation="5">
                                <div class="d-flex align-center justify-space-between">
                                    <div class="">
                                        <h2>B.Sc in Computer Science & Engineering</h2>
                                        <span>March 2015 - Octaber 2019</span>
                                    </div>
                                    <a class="green--text">at World University <v-icon color="green">mdi-link</v-icon></a>
                                </div>
                                <v-card-text>
                                    <v-list>
                                       <v-list-item>
                                          <v-list-item-content>
                                            <v-list-item-title>CGPA: 3.34</v-list-item-title>
                                          </v-list-item-content>
                                        </v-list-item>

      <v-list-item>
        <v-list-item-content>
          <v-list-item-subtitle>Active Competitive Programmer in programming Society</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-list>

                                </v-card-text>
                            </v-card>
                        </v-col>
                        <v-col cols="12" lg="6">
                            <v-card class="pa-6 rounded-xl " elevation="5">
                                <div class="d-flex align-center justify-space-between">
                                    <div class="">
                                        <h2>Higher Secondary Certificate, Dhaka</h2>
                                        <span>May 2013 - Aug 2014</span>
                                    </div>
                                    <a class="green--text">at College of Metropolis Degree College<v-icon color="green">mdi-link</v-icon></a>
                                </div>
                                <v-card-text>
                                    <v-list>
                                       <v-list-item>
                                          <v-list-item-content>
                                            <v-list-item-title>GPA: 3.90</v-list-item-title>
                                          </v-list-item-content>
                                        </v-list-item>

                                        <v-list-item>
                                          <v-list-item-content>
                                            <v-list-item-title>Science and Mathematics</v-list-item-title>
                                          </v-list-item-content>
                                        </v-list-item>
                                      </v-list>
                                </v-card-text>
                            </v-card>
                        </v-col>
                    </v-row>
                </v-container>
            </section>
            <section class="contact-us pt-10">
                <v-img class="pt-10" gradient="to bottom, rgb(166 199 156), rgb(227 227 227 / 86%)" src="@/assets/images/contact-us.webp">
                    <v-container>
                        <h4 class="display-1 text-center mb-5">
                            I’m a Backend Developer, based in Web and Mobile Application. Currently a freelancer. 
                        </h4>
                        <v-divider />
                        <br>
                        <v-row>
                            <v-col cols="12" lg="6">
                                <v-card-title>DROP A LINE</v-card-title>
                                <v-form>
                                    <v-text-field label="Your Name" />
                                    <v-text-field label="Email" />
                                    <v-text-field label="Subject" />
                                    <v-textarea label="Message" />
                                    <v-btn large color="green" class="white--text">Send Message</v-btn>
                                </v-form>
                            </v-col>
                            <v-col cols="12" lg="3" offset="2">
                                <v-card-title>CONTACT ME</v-card-title>
                                <v-card-text>
                                    47, East Islambag, Lalbag, Dhaka-1211 <br>
                                    +88-01515656106 <br>
                                    kawserahmed954@gmail.com <br>
                                </v-card-text>
                                <v-card-actions>
                                    <v-btn large elevation="5" color="pink" class="white--text mt-10 px-10 py-5">Download
                                        Resume
                                        <v-icon>mdi-download</v-icon>
                                    </v-btn>
                                </v-card-actions>
                            </v-col>
                        </v-row>
                    </v-container>
                    <v-footer class="mt-4">
                        <v-col
                                class="text-center"
                                cols="12"
                        >
                            <strong>Copyright ©{{ new Date().getFullYear() }} All rights reserved | This is made by
                                <a href="" class="green--text">kawsarahmed@954</a>
                            </strong>
                        </v-col>
                    </v-footer>
                </v-img>
            </section>
    </v-main>
  </v-app>

</template>

<script>

export default {
  name: 'App',

 

  data: () => ({
    drawer: null,
    items: [
              {title: 'HTML', value: 100, color: 'light-blue'},
              {title: 'CSS', value: 100, color: 'deep-orange'},
              {title: 'Javascript', value: 70, color: 'light-green'},
              {title: 'Vuejs', value: 50, color: 'blue'},
              {title: 'Python', value: 90, color: 'black'},
              {title: 'Dart', value: 70, color: 'red'},
              {title: 'flutter', value: 70, color: 'purple'},
            ],
  }),
};
</script>



