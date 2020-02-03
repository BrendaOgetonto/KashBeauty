<template>
  <div>
    <div class="page-header page-header-small">
      <parallax
        class="page-header-image"
        style="background-image: url('img/makeup_brushes.jpg')"
      >
      </parallax>
      <div class="content-center">
        <div class="container">
          <h1 class="title">Kash Beauty.</h1>
          <div class="text-center">
            <a href="#pablo" class="btn btn-primary btn-icon btn-round">
              <i class="fab fa-facebook-square"></i>
            </a>
            <a href="#pablo" class="btn btn-primary btn-icon btn-round">
              <i class="fab fa-twitter"></i>
            </a>
            <a href="#pablo" class="btn btn-primary btn-icon btn-round">
              <i class="fab fa-google-plus"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="section section-about-us">
      <div class="container">
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h2 class="title">What is Kash Beauty?</h2>
            <h5 class="description">
            Kash Beauty is a beauty brand that not only brings out your physical beauty but also you inner beauty. 
            Founded by Kamene Kyalo, a lawyer and soon to be advocate, 
            her passion for beauty has allowed her to also expand and deliver legal services in the beauty industry. 
            We deliver services in Bridal, Photoshoots,  Runway and Editorial events. 
            Its either a whole lot of glam and law.
            </h5>
          </div>
        </div>
        <div class="separator separator-primary"></div>
        <div class="section-story-overview">
          <div class="row">
            <div class="col-md-6">
              <div
                class="image-container image-left"
                style="background-image: url('img/kash2.jpg')"
              >
                <!-- First image on the left side -->
                <p class="blockquote blockquote-primary">
                  "I believe that all women are pretty without makeup, but with the right makeup can be pretty powerful "
                  <br />
                  <br />
                  <small>-Bobby Brown</small>
                </p>
              </div>
            </div>
            <div class="col-md-5">
              <!-- First image on the right side, above the article -->
              <div
                class="image-container image-right"
                style="background-image: url('img/kash.jpg')"
              ></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- carousel -->
    <div class="col-md-6 ml-auto mr-auto">
            <h4 class="title text-center">My Portfolio</h4>
          </div>
    <tabs pills
            class="nav-align-center"
            tab-content-classes="gallery"
            tab-nav-classes="nav-pills-just-icons"
            type="primary">
      <tab-pane label="SFX">
        <i slot="label">SFX</i>
        <div class="section" id="carousel">
          <div class="container">
            <!-- <div class="title">
              <h4>SFX</h4>
            </div> -->
            <div class="row justify-content-center">
              <div class="col-8">
                <el-carousel height="500px">
                  <el-carousel-item  margin="auto">
                    <img class="d-block" src="img/sfx/img1.jpg" alt="" width="50%" margin="auto" left="40px"/>
                  </el-carousel-item>
                  <el-carousel-item>
                    <img class="d-block" src="img/sfx/img2.jpg" alt="" height="100%" width="50%"/>
                  </el-carousel-item>
                </el-carousel>
              </div>
            </div>
          </div>
      </div>
    </tab-pane>
    <tab-pane label="Random">
        <i slot="label">Random</i>
          <div class="section" id="carousel">
            <div class="container">
              <!-- <div class="title">
                <h4>Folder 1</h4>
              </div> -->
              <div class="row justify-content-center">
                <div class="col-8">
                  <el-carousel height="500px">
                    <el-carousel-item>
                      <img class="d-block" src="img/folder1/img1.jpg" alt="First slide" height="100%" width="50%"/>
                    </el-carousel-item>
                    <el-carousel-item>
                      <img class="d-block" src="img/folder1/img2.jpg" alt="Second slide" height="100%" width="50%"/>
                    </el-carousel-item>
                    <el-carousel-item>
                      <img class="d-block" src="img/folder1/img3.jpg" alt="Third slide" height="100%" width="50%"/>
                    </el-carousel-item>
                  </el-carousel>
                </div>
              </div>
          </div>
        </div>
    </tab-pane>
    <tab-pane label="Bridal">
        <i slot="label">Bridal</i>
          <div class="section" id="carousel">
            <div class="container">
              <!-- <div class="title">
                <h4>Folder 2</h4>
              </div> -->
              <div class="row justify-content-center">
                <div class="col-8">
                  <el-carousel height="500px" >
                    <el-carousel-item>
                      <img class="d-block" src="img/folder2/img1.jpg" alt="First slide" height="100%" width="50%"/>
                    </el-carousel-item>
                    <el-carousel-item>
                      <img class="d-block" src="img/folder2/img2.jpg" alt="Second slide" height="100%" width="50%"/>
                    </el-carousel-item>
                    <el-carousel-item>
                      <img class="d-block" src="img/folder2/img3.jpg" alt="Third slide" height="100%" width="50%"/>
                    </el-carousel-item>
                  </el-carousel>
                </div>
              </div>
            </div>
        </div>
    </tab-pane>
    </tabs>
          <!-- end carousel -->
    <div class="section section-contact-us text-center">
      <div class="container">
        <h2 class="title">Want to work with us?</h2>
        <p class="description">Your project is very important to us.</p>
        <div class="row">
          <div class="col-lg-6 text-center ml-auto mr-auto col-md-8">
            <fg-input
              class="input-lg"
              placeholder="First Name..."
              v-model="form.firstName"
              addon-left-icon="now-ui-icons users_circle-08"
            >
            </fg-input>
            <fg-input
              class="input-lg"
              placeholder="Email Here..."
              v-model="form.email"
              addon-left-icon="now-ui-icons ui-1_email-85"
            >
            </fg-input>
            <div class="textarea-container">
              <textarea
                class="form-control"
                name="name"
                rows="4"
                cols="80"
                v-model="form.message"
                placeholder="Type a message..."
              ></textarea>
            </div>
            <div class="send-button">
              <n-button type="primary" round block size="lg"
                >Send Message</n-button
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { Button, FormGroupInput } from '@/components';
import { Tabs, TabPane } from '@/components';
import { Carousel, CarouselItem } from 'element-ui';

export default {
  name: 'about',
//   bodyClass: 'landing-page',
  components: {
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput,
    [Carousel.name]: Carousel,
    [CarouselItem.name]: CarouselItem,
    Tabs,
    TabPane
  },
  data() {
    return {
      form: {
        firstName: '',
        email: '',
        message: '',
      },
      images:[]
    };
  }
};

</script>
<style></style>
