<template>
  <v-container>
    <v-row class="mx-auto my-16" style="max-width: 90%;">
      <v-col cols="12" sm="6" md="6">
        <v-card data-aos="fade-up" data-aos-duration="1500"
          :disabled="loading"
          :loading="loading"
          class="mx-auto"
          max-width="100%"
          style=" color: #000; background-color: transparent; border-radius: 0; box-shadow: none;"
        >
          <template v-slot:loader="{ isActive }">
            <v-progress-linear
              :active="isActive"
              color="deep-purple"
              height="4"
              indeterminate
            ></v-progress-linear>
          </template>

          <v-img
            src="../assets/pic_1.jpg"
            height="350"
            cover
            style=""
          ></v-img>

          <v-card-item>
            <v-card-title style="
                text-align: left;
                color: #000;
                font-size: 1.6vw;
                font-weight: 900;
                margin-bottom: 1vw;
                position: relative;
            " >
              <span style="color: #999;">01.&emsp;</span>
              <span style="color: #000;">
                Business Setup
              </span>
            </v-card-title>
          </v-card-item>

          <v-card-text style="
                  text-align: left;
                  color: #555;
                  font-size: 1.1vw;
                  line-height: 150%;
                  font-weight: 400;
              ">
            <div>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</div>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" sm="6" md="6">
        <v-card data-aos="fade-up" data-aos-duration="1500"
          :disabled="loading"
          :loading="loading"
          class="mx-auto"
          max-width="100%"
          style=" color: #000; background-color: transparent; border-radius: 0; box-shadow: none;"
        >
          <template v-slot:loader="{ isActive }">
            <v-progress-linear
              :active="isActive"
              color="deep-purple"
              height="4"
              indeterminate
            ></v-progress-linear>
          </template>

          <v-img
            src="../assets/pic_2.jpg"
            height="350"
            cover
            style=""
          ></v-img>

          <v-card-item>
            <v-card-title style="
                text-align: left;
                color: #000;
                font-size: 1.6vw;
                font-weight: 900;
                margin-bottom: 1vw;
                position: relative;
            " >
              <span style="color: #999;">02.&emsp;</span>
              <span style="color: #000;">
                Digital Transformation
              </span>
            </v-card-title>
          </v-card-item>

          <v-card-text style="
                  text-align: left;
                  color: #555;
                  font-size: 1.1vw;
                  line-height: 150%;
                  font-weight: 400;
              ">
            <div>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</div>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" sm="6" md="6">
        <v-card data-aos="fade-up" data-aos-duration="1500"
          :disabled="loading"
          :loading="loading"
          class="mx-auto"
          max-width="100%"
          style=" color: #000; background-color: transparent; border-radius: 0; box-shadow: none;"
        >
          <template v-slot:loader="{ isActive }">
            <v-progress-linear
              :active="isActive"
              color="deep-purple"
              height="4"
              indeterminate
            ></v-progress-linear>
          </template>

          <v-img
            src="../assets/pic_3.jpg"
            height="350"
            cover
            style=""
          ></v-img>

          <v-card-item>
            <v-card-title style="
                text-align: left;
                color: #000;
                font-size: 1.6vw;
                font-weight: 900;
                margin-bottom: 1vw;
                position: relative;
            " >
              <span style="color: #999;">03.&emsp;</span>
              <span style="color: #000;">
                Data Science
              </span>
            </v-card-title>
          </v-card-item>

          <v-card-text style="
                  text-align: left;
                  color: #555;
                  font-size: 1.1vw;
                  line-height: 150%;
                  font-weight: 400;
              ">
            <div>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</div>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" sm="6" md="6">
        <v-card data-aos="fade-up" data-aos-duration="1500"
          :disabled="loading"
          :loading="loading"
          class="mx-auto"
          max-width="100%"
          style=" color: #000; background-color: transparent; border-radius: 0; box-shadow: none;"
        >
          <template v-slot:loader="{ isActive }">
            <v-progress-linear
              :active="isActive"
              color="deep-purple"
              height="4"
              indeterminate
            ></v-progress-linear>
          </template>

          <v-img
            src="../assets/pic_4.jpg"
            height="350"
            cover
            style=""
          ></v-img>

          <v-card-item>
            <v-card-title style="
                text-align: left;
                color: #000;
                font-size: 1.6vw;
                font-weight: 900;
                margin-bottom: 1vw;
                position: relative;
            " >
              <span style="color: #999;">04.&emsp;</span>
              <span style="color: #000;">
                Customer Support
              </span>
            </v-card-title>
          </v-card-item>

          <v-card-text style="
                  text-align: left;
                  color: #555;
                  font-size: 1.1vw;
                  line-height: 150%;
                  font-weight: 400;
              ">
            <div>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</div>
          </v-card-text>
        </v-card>
      </v-col>


    </v-row>
  </v-container>  
</template>

<script>
import AOS from 'aos'
import 'aos/dist/aos.css'
import { gsap } from 'gsap'
import { ScrollTrigger } from 'gsap/ScrollTrigger'
gsap.registerPlugin(ScrollTrigger)
AOS.init({
  once: true
})

  export default {
    data: () => ({
      loading: false,
      selection: 1,
    }),

    methods: {
      reserve () {
        this.loading = true

        setTimeout(() => (this.loading = false), 1000)
      },
    },
  }
</script>
