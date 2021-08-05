<template>
  <div class="wrapper">
    <parallax class="page-header header-filter" :style="headerStyle">
      <div class="md-layout">
        <div class="md-layout-item">
          <div class="image-wrapper">
            <!-- <img :src="leaf4" alt="leaf4" class="leaf4" v-show="leafShow" /> -->

            <div class="brand">
              <h1>Computer Science</h1>
              <h3>Maejo University</h3>
            </div>
          </div>
        </div>
      </div>
    </parallax>

    <div class="main main-raised">

      <div class="section">
        <div class="container">
           <div class="title">
            <h2>News & Information</h2>
            <h4>ข่าวสารประชาสัมพันธ์ข้อมูล</h4>
          </div>

          <hr>

          <div class="md-layout">
            <div class="md-layout-item  mx-auto md-small-size-100">
              <md-card>
                <carousel
                  :per-page="1"
                  loop
                  :speed="700"
                  autoplay
                  :autoplay-timeout="5000"
                  :mouse-drag="false"
                  navigationEnabled
                  navigationNextLabel="<i class='material-icons'>keyboard_arrow_right</i>"
                  navigationPrevLabel="<i class='material-icons'>keyboard_arrow_left</i>"
                >
                  <slide>
                    <div class="carousel-caption">
                      <h4>
                        <md-icon>location_on</md-icon>
                        Somewhere Beyond, United States
                      </h4>
                    </div>
                    <img :src="carousel1" alt="carousel1" />
                  </slide>
                  <slide>
                    <div class="carousel-caption">
                      <h4>
                        <md-icon>location_on</md-icon>
                        Yellowstone National Park, United States
                      </h4>
                    </div>
                    <img :src="carousel2" alt="carousel2" />
                  </slide>
                  <slide>
                    <div class="carousel-caption">
                      <h4>
                        <md-icon>location_on</md-icon>
                        Yellowstone National Park, United States
                      </h4>
                    </div>
                    <img :src="carousel3" alt="carousel3" />
                  </slide>
                </carousel>
              </md-card>
            </div>
          </div>

          <div class="row row-cols-1 row-cols-md-2 g-4">
            <div class="col">
              <div class="card">
                <img
                  src="@/assets/img/header.jpg"
                  class="card-img-top"
                  alt="..."
                />
                <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">
                    This is a longer card with supporting text below as a
                    natural lead-in to additional content. This content is a
                    little bit longer.
                  </p>
                </div>
              </div>
            </div>
            <div class="col">
              <div class="card">
                <img
                  src="@/assets/img/header.jpg"
                  class="card-img-top"
                  alt="..."
                />
                <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">
                    This is a longer card with supporting text below as a
                    natural lead-in to additional content. This content is a
                    little bit longer.
                  </p>
                </div>
              </div>
            </div>
          </div>
          <br />
          <div class="row row-cols-1 row-cols-md-3 g-4">
            <div class="col">
              <div class="card h-100">
                <img
                  src="@/assets/img/header.jpg"
                  class="card-img-top"
                  alt="..."
                />
                <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">
                    This is a wider card with supporting text below as a natural
                    lead-in to additional content. This content is a little bit
                    longer.
                  </p>
                </div>
              </div>
            </div>
            <div class="col">
              <div class="card h-100">
                <img
                  src="@/assets/img/header.jpg"
                  class="card-img-top"
                  alt="..."
                />
                <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">
                    This card has supporting text below as a natural lead-in to
                    additional content.
                  </p>
                </div>
              </div>
            </div>
            <div class="col">
              <div class="card h-100">
                <img
                  src="@/assets/img/header.jpg"
                  class="card-img-top"
                  alt="..."
                />
                <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">
                    This is a wider card with supporting text below as a natural
                    lead-in to additional content. This card has even longer
                    content than the first to show that equal height action.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="section">
        <div class="container">
          <div class="title">
            <h2>Course Outline</h2>
            <h4>หลักสูตรการเรียน</h4>
          </div>
          <md-datepicker v-model="selectedDate">
                <label>Select date</label>
              </md-datepicker>
        </div>
      </div>

      <div class="section">
        <div class="container">
          <div class="title">
            <h2>Workshop & Activity</h2>
            <h4>ภาพกิจกรรมและอบรม</h4>
          </div>
        </div>
      </div>

         <div class="section">
        <div class="container">
          <div class="title">
            <h2>Introduction</h2>
            <h4>วิดีโอประชาสัมพันธ์หลักสูตร</h4>
          </div>
          <div class="">
        <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/88JeU0ShY60?controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </div>

        

     

         
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  components: {},
  name: "index",
  bodyClass: "index-page",
  props: {
    image: {
      type: String,
      default: require("@/assets/img/header.jpg"),
    },
    leaf4: {
      type: String,
      default: require("@/assets/img/leaf4.png"),
    },
    leaf3: {
      type: String,
      default: require("@/assets/img/leaf3.png"),
    },
    leaf2: {
      type: String,
      default: require("@/assets/img/leaf2.png"),
    },
    leaf1: {
      type: String,
      default: require("@/assets/img/leaf1.png"),
    },
    signup: {
      type: String,
      default: require("@/assets/img/city.jpg"),
    },
    landing: {
      type: String,
      default: require("@/assets/img/landing.jpg"),
    },
    profile: {
      type: String,
      default: require("@/assets/img/profile.jpg"),
    },
  },
  data() {
    return {
      carousel1: require("@/assets/img/header.jpg"),
      carousel2: require("@/assets/img/header.jpg"),
      carousel3: require("@/assets/img/header.jpg"),

      firstname: null,
      email: null,
      password: null,
      leafShow: false,
    };
  },
  methods: {
    leafActive() {
      if (window.innerWidth < 768) {
        this.leafShow = false;
      } else {
        this.leafShow = true;
      }
    },
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.image})`,
      };
    },
    signupImage() {
      return {
        backgroundImage: `url(${this.signup})`,
      };
    },
  },
  mounted() {
    this.leafActive();
    window.addEventListener("resize", this.leafActive);
  },
  beforeDestroy() {
    window.removeEventListener("resize", this.leafActive);
  },
};
</script>

<style lang="scss">
.section-download {
  .md-button + .md-button {
    margin-left: 5px;
  }
}

@media all and (min-width: 991px) {
  .btn-container {
    display: flex;
  }
}
</style>
