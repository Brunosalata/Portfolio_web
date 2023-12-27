<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-grey">Hello,</h1>
              <h1 class="text-white">I'm Bruno Salata</h1>
              <span class="text-grey">Systems and Web Pages Designer & Developer</span><br />
              <v-btn tile dark class="text-yellow mt-8" variant="outlined">Contact me</v-btn>
            </div>
          </v-col>
          <v-col cols="2"></v-col>
          <div style="position: absolute; z-index: 9999; bottom: 0; margin-left:auto; margin-right: auto; left: 0; right: 0; text-align: center;">
            <v-icon>fas fa-angle-double-down</v-icon>
          </div>
          <v-col cols="5">
            <div style="position: relative; z-index: 9999;" class="mt-16">
              <v-img src="https://static.vecteezy.com/system/resources/previews/010/869/739/large_2x/file-management-concept-illustration-modern-concept-of-file-management-system-online-document-storage-service-free-png.png" contain max-height="300"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" class="mt-16" id="about">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="https://static.vecteezy.com/system/resources/previews/023/477/459/non_2x/ai-generative-cartoon-laptop-with-books-free-png.png" max-height="300"></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
              <h5 class="mt-16">About Me</h5>
              <div style="width: 120px">
                <v-slider v-model="slider" color="yellow" label="track-color">

                </v-slider>
              </div>
              <h4 class="mt-n4">I'm a Creative Java System Designer</h4>
              <h4>Working on Web Development too</h4>
              <p class="text-grey">Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
                Esse possimus quam quod architecto eligendi incidunt, neque consectetur inventore 
                nesciunt excepturi perspiciatis, tenetur delectus! Facilis quasi ad corporis, 
                dolores nobis cupiditate.</p>
            <br />
            <p class="text-grey">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa 
              nam cum impedit illum quod praesentium vel, neque eligendi repellat dolorem ipsam a, 
              vero animi inventore expedita voluptatem ex! Inventore, quis.</p>
            <v-btn tile dark color="yellow" class="mt-4">
              Download Resume
            </v-btn>
          </v-col>
          </v-row>
        </div>
      </v-col>
      <div class="text-center mt-4">
        <h2>What We Do</h2>
        <div style="width: 120px; margin: 0 auto">
          <v-slider v-model="slider" color="yellow" label="track-color">
          </v-slider>
        </div>
      </div>
      <v-col cols="12" class="padd" id="portfolio">
        <div class="first" id="project">
          <v-row>
            <v-col cols="12">
              <div class="child">
                <v-btn icon="fas fa-laptop" color="#fbdf7e" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Web Design</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet consectetur,<br /> adipisicing elit. Eos doloremque.<br />
                </p>
              </div>
              <div class="child">
                <v-btn icon="fas fa-mobile-alt" color="#fbdf7e" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">System Develop</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet<br /> consectetur, adipisicing elit.<br /> Eos doloremque alias.<br />
                </p>
              </div>
              <div class="child">
                <v-btn icon="fas fa-location" color="#fbdf7e" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Branding</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet<br /> consectetur, adipisicing<br /> elit. Eos doloremque.<br />
                </p>
              </div>
            </v-col>
          </v-row>
          <v-divider></v-divider>
        </div>
      </v-col>
      <v-col cols="12" sm="12" id="services">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#fbdf7e" class="mr-2">All</v-btn>
          <v-btn class="mr-2" variant="tonal">Desktop System</v-btn>
          <v-btn class="mr-2" variant="tonal">Web Design</v-btn>
          <v-btn class="mr-2" variant="tonal">Branding</v-btn>
          <v-btn variant="tonal">Courses</v-btn>
        </div>
      </v-col>
      <v-col cols="12" class="imgHover">
        <v-row class="fill-height" align:="center" justify="center">
          <template v-for="(item, i) in items" :key="i">
            <v-col cols="12" md="4">
              <v-hover v-slot="{isHovering, props}">
                <v-card :elevation="isHovering ? 12: 2" :class="{'on-hover' : isHovering}" v-bind="props">
                  <v-img :src="item.img" height="225px" cover></v-img>
                </v-card>
              </v-hover>
            </v-col>
          </template>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#fbdf7e" class="mt-4">Load More</v-btn>
        </div>
      </v-col>
      <v-col cols="12" id="page">
        <div class="pre">
          <v-row>
            <v-col cols="12" sm="4">
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="https://securityintelligence.com/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2020/10/Web-Application-Security-Best-Practices-.jpeg.webp" height="200px" cover></v-img>
                <v-card-title>We provide you the best</v-card-title>
                <v-card-subtitle>By Bruno Salata | 26 dec 2023</v-card-subtitle>
                <v-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit.</v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="https://images.pexels.com/photos/1181336/pexels-photo-1181336.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" height="200px" cover></v-img>
                <v-card-title>We provide you the best</v-card-title>
                <v-card-subtitle>By Bruno Salata | 26 dec 2023</v-card-subtitle>
                <v-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit.</v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="https://images.pexels.com/photos/1181473/pexels-photo-1181473.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" height="200px" cover></v-img>
                <v-card-title>We provide you the best</v-card-title>
                <v-card-subtitle>By Bruno Salata | 26 dec 2023</v-card-subtitle>
                <v-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit.</v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" id="blog">
        <div class="hire">
          <v-row>
            <v-col cols="12" sm="8">
              <h1 class="mt-9">Hire me for your next project</h1>
              <p class="text-grey">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nihil, magni ipsum! Accusantium recusandae
              </p>
            </v-col>
            <v-col cols="12" sm="4">
              <v-btn color="#fbdf7e" class="mt-15">Hire Me</v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" sm="12" class="px-16" id="contact">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="child">
              <h1>Contact info.</h1>
              <v-btn icon="fas fa-map-marker-alt" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">Your Street SYO, Your Area Dream</span><br />
              <v-btn icon="fas fa-phone-alt" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">(16) 99127-8804</span><br />
              <span class="text-caption">(16) 99127-8804</span><br />
              <v-btn icon="fas fa-envelope" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">brunoslima@gmail.com</span><br />
            </div>
          </v-col>
          <v-col cols="12" sm="8">
            <h1 class="mt-8">Send your message</h1>
            <v-divider></v-divider>
            <span class="text-caption">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minima repellendus magni quam maiores, 
              illum assumenda fuga nemo deserunt tempora rem aliquid quae odio iste similique ipsa! Dignissimos, 
              accusamus. Similique, officia?
            </span>
            <v-row class="mt-10">
              <v-col cols="12" sm="6">
                <v-text-field label="Name" persistent-hint variant="outlined"></v-text-field>
              </v-col>
              <v-col cols="12" sm="6">
                <v-text-field label="Phone Number" persistent-hint variant="outlined"></v-text-field>
              </v-col>
            </v-row>
            <v-textarea label="Message" persistent-hint variant="outlined"></v-textarea>
            <v-btn color="#fbdf7e" class="mt-2">Submit Now</v-btn>
          </v-col>
        </v-row>
      </v-col>
    </v-container>
    <FooterView />
  </v-app>
</template>

<script >
import { defineComponent } from 'vue';

// Component
import NavBar from '@/components/NavBar.vue';
import FooterView from '@/components/FooterView.vue';

export default defineComponent({
  name: 'HomeView',
  setup(){
    return {
      slider: 50,

      items: [
          {
            img: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          },
          {
            img: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            img: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          },
          {
            img: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          },
        ],
    }
  },

  components: {
      NavBar,
      FooterView,
  },
});
</script>

<style>
.v-container{
  padding: 16px 0;
}
.head{
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width: 100%;
  color: white;
}
.head:before{
  content: " ";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}
.head:after{
  content: " ";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}
.egg{
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 356px;
  height: 300px;
  background-color: #fbdf7e;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 0%;
}
.first{
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 2rem 2rem;
}
.child{
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}
.imgHover{
  padding: 0 200px;
}
.pre{
  width: 100%;
  height: 380px;
  text-align: center;
  padding: 0 200px;
  background-color: #f5f5f5;
}
.hire{
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #e9e9e9;
  margin-top: -24px;
}
</style>
