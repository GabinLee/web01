<template>
  <div class="home">
    <header id="header">
      <div class="h-container">
        <div class="logo-box">
          <a href="/">
            <p>SAMPLE</p>
          </a>
        </div>
        
        <nav class="nav-box fs16">
          <div class="nav-group">
            <div class="nav-item">
              <button @click="moveAbout(1)" :class="{ active : selectedNav == 1 ? true : false }">about</button>
            </div>
            <div class="nav-item">
              <button @click="moveServices(2)" :class="{ active : selectedNav == 2 ? true : false }">services</button>
            </div>
            <div class="nav-item">
              <button @click="moveProjects(3)" :class="{ active : selectedNav == 3 ? true : false }">projects</button>
            </div>
          </div>
          
        </nav>

        <div class="mobile-menu-btn-box">
          <v-app-bar-nav-icon @click="openMobileNav" />
        </div>
      </div>

      <div class="mobile-nav-box fs20" id="mobile-nav-box">
        <div class="group" id="group">
          <div class="close-item">
            <button v-ripple @click="closeMobileNav">
              <v-icon>mdi-close</v-icon>
            </button>
          </div>
          <div class="nav-item" v-ripple>
            <button @click="moveAbout">about</button>
          </div>
          <div class="nav-item" v-ripple>
            <button @click="moveServices">services</button>
          </div>
          <div class="nav-item" v-ripple>
            <button @click="moveProjects">projects</button>
          </div>
        </div>
      </div>
    </header>

    <main>
      <div class="intro">
        <div class="bg-grey text-center">
          <div class="text-box">
            <h1 class="uppercase fs60">sample</h1>
            <hr>
            <p class="j-title">Sample - You can change this text.</p>
          </div>
        </div>
      </div>

      <div class="about" id="about">
        <div class="inner-box mw1280">
          <div class="group" data-aos="fade-right">
            <div class="text-box">
              <div class="j-head">
                <span>about our company</span>
              </div>
              <div class="contents j-text">
                <p>You can change this text</p>
                <p>You can change this text</p>
                <p>You can change this text</p>
                <p>You can change this text</p>
                <p>You can change this text</p>
              </div>
            </div>
            <div class="img-box">
              <img src="../assets/about1.jpg" alt="">
            </div>
          </div>

          <div class="group history" data-aos="fade-left">
            <div class="img-box">
              <img src="../assets/about2.jpg" alt="">
            </div>
            <div class="text-box">
              <div class="j-head">
                <span>company history</span>
              </div>
              <div class="contents j-text">
                <p><strong class="j-title">2020</strong>You can change this text</p>
                <p><strong class="j-title">2019</strong>You can change this text</p>
                <p><strong class="j-title">2018</strong>You can change this text</p>
                <p><strong class="j-title">2017</strong>You can change this text</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="services" id="services">
        <div class="bg-grey">
          <div class="inner-box mw1280">
            <h1 class="text-center fs36">Our Services</h1>
            <hr>
            <div class="group">
              <div class="con-box">
                <div class="icon-box">
                  <v-icon>mdi-cellphone-iphone</v-icon>
                </div>
                <div class="text-box">
                  <p class="j-title">Title</p>
                  <p class='j-text'>You can change this text</p>
                </div>
              </div>

              <div class="con-box">
                <div class="icon-box">
                  <v-icon>mdi-laptop-mac</v-icon>
                </div>
                <div class="text-box">
                  <p class="j-title">Title</p>
                  <p class='j-text'>You can change this text</p>
                </div>
              </div>

              <div class="con-box">
                <div class="icon-box">
                  <v-icon>mdi-monitor-cellphone</v-icon>
                </div>
                <div class="text-box">
                  <p class="j-title">Title</p>
                  <p class='j-text'>You can change this text</p>
                </div>
              </div>

              <div class="con-box">
                <div class="icon-box">
                  <v-icon>mdi-cellphone-iphone</v-icon>
                </div>
                <div class="text-box">
                  <p class="j-title">Title</p>
                  <p class='j-text'>You can change this text</p>
                </div>
              </div>

              <div class="con-box">
                <div class="icon-box">
                  <v-icon>mdi-cellphone-iphone</v-icon>
                </div>
                <div class="text-box">
                  <p class="j-title">Title</p>
                  <p class='j-text'>You can change this text</p>
                </div>
              </div>

              <div class="con-box">
                <div class="icon-box">
                  <v-icon>mdi-cellphone-iphone</v-icon>
                </div>
                <div class="text-box">
                  <p class="j-title">Title</p>
                  <p class='j-text'>You can change this text</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      
      <div class="projects" id="projects">
        <div class="inner-box mw1280">
          <div class="j-head"><span>projects</span></div>
          <div class="group">
            <div class="card-box" data-aos="fade-up">
              <img src="../assets/projects1.jpg" alt="">
              <div class="text-box">
                <p class="j-title">Title</p>
                <p class="j-text">You can change this text</p>
              </div>
            </div>

            <div class="card-box" data-aos="fade-up">
              <img src="../assets/projects2.jpg" alt="">
              <div class="text-box">
                <p class="j-title">Title</p>
                <p class="j-text">You can change this text</p>
              </div>
            </div>

            <div class="card-box" data-aos="fade-up">
              <img src="../assets/projects3.jpg" alt="">
              <div class="text-box">
                <p class="j-title">Title</p>
                <p class="j-text">You can change this text</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>

    <footer>
      <div class="f-container mw1280">
        <div class="group">
          <div class="info-box">
            <p class="j-title uppercase">call</p>
            <p class="j-text">000-0000-0000</p>
          </div>
          <div class="info-box">
            <p class="j-title uppercase">e-mail</p>
            <p class="j-text">happy@jollybeen.com</p>
          </div>
          <div class="info-box">
            <p class="j-title uppercase">address</p>
            <p class="j-text">Seoul</p>
          </div>
          <div class="info-box">
            <p class="j-title uppercase">find me</p>
            <p class="j-text">instagram</p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data: () => ({
    selectedNav : 0
  }),
  created() {
    window.onscroll = function () {
      if (document.body.scrollTop > 0.1 || document.documentElement.scrollTop > 0.1) {
        document.getElementById("header").classList.add('scroll-header')
      } else{
        document.getElementById("header").classList.remove('scroll-header')
      }
    }
    // window.onload = function() {
    //   setTimeout(function() {
    //     scrollTo(0,0);
    //   }, 100);
      
    // }
  },
  mounted() {
    console.log(document.getElementById("about").offsetTop)
    // console.log(document.getElementById("projects-container").offsetTop)
    // console.log(document.getElementById("contact-container").offsetTop)
    window.addEventListener('scroll', () => {
      if(window.scrollY < 652) {
        this.selectedNav = 0
      } else if(window.scrollY < 1397) {
        this.selectedNav = 1
      } else if(window.scrollY < 1840) {
        this.selectedNav = 2
      } else {
        this.selectedNav = 3
      }
    })
  },
  methods: {
    openMobileNav() {
      document.getElementById("mobile-nav-box").style.width = "100%";
      document.getElementById("group").style.width = "50%";
    },
    closeMobileNav() {
      document.getElementById("mobile-nav-box").style.width = "0%";
      document.getElementById("group").style.width = "0%";
    },
    moveAbout(index) {
      this.selectedNav = index;
      if(window.innerWidth < 701 ) {
        window.scroll({
          top: document.getElementById("about").offsetTop + -60,
          behavior: 'smooth'
        })
      } else {
        window.scroll({
          top: document.getElementById("about").offsetTop + -80,
          behavior: 'smooth'
        })  
      }
      this.closeMobileNav();
    },
    moveServices(index) {
      this.selectedNav = index;
      if(window.innerWidth < 701 ) {
        window.scroll({
          top: document.getElementById("services").offsetTop + -60,
          behavior: 'smooth'
        })
      } else {
        window.scroll({
          top: document.getElementById("services").offsetTop + -80,
          behavior: 'smooth'
        })
      }
      this.closeMobileNav();
    },
    moveProjects(index) {
      this.selectedNav = index;
      if(window.innerWidth < 701 ) {
        window.scroll({
          top: document.getElementById("projects").offsetTop + -60,
          behavior: 'smooth'
        })
      } else {
        window.scroll({
          top: document.getElementById("projects").offsetTop + -80,
          behavior: 'smooth'
        })
      }
      this.closeMobileNav();
    }
  }
}
</script>


<style lang="scss" scoped>
  .home{ overflow: hidden; }
  .theme--light.v-btn.v-btn--icon{ color: #000; }
  hr{
    background-color: #1BB850;
    height: 4px;
    margin: 20px auto 40px;
    border: none;
  }
  
  /* header */
    header{
      background-color: transparent;
      width: 100%;
      height: 80px;
      position: fixed;
      z-index: 999;
    }
    .h-container{
      height: inherit;
      max-width: 1280px;
      margin: 0 auto;
      padding: 0 40px;
      display: flex;
      justify-content: space-between;
      position: relative;
    }
    .logo-box{
      height: inherit;
      a{
        height: inherit;
        display: flex;
        align-items: center;
      }
      p{
        color: #1BB850;
        font-size: 36px;
        margin: 0;
      }
    }

    .nav-group{
      display: flex;

      .nav-item{
        margin-left: 40px;

        button{
          color: #fff;
          height: 80px;
          line-height: 80px;
          text-transform: uppercase;
          letter-spacing: 0.05em;
          position: relative;
        }
        button:before{
          content: "";
          position: absolute;
          width: 0;
          height: 2px;
          bottom: 26px;
          left: 50%;
          background: #1BB850;
          transform: translate(-50%, 0%);
          transition: .2s;
        }
        button:hover:before, .active::before{ width: 100%; }
      }
      .nav-item:nth-child(1){
        margin-left: 0;
      }
    }

    .mobile-menu-btn-box{
      display: none;

      .v-btn--icon.v-size--default{
        color: #1BB850;
        width: 40px;
        height: 40px;
        margin: 20px 0;
        .v-icon{
          color: #fff;
          width: 30px;
          height: 30px;
          font-size: 30px;
        }
      }
    }

    .mobile-nav-box{
      background-color: rgba(0, 0, 0, .8);
      width: 0;
      height: 100vh;
      overflow: hidden;
      position: absolute;
      top: 0;
      right: 0;
      display: flex;
      justify-content: space-between;

      .group{
        background-color: #fff;
        width: 0%;
        transition: .5s;
        margin-left: auto;

        .close-item{
          height: 80px;
          padding: 20px 40px;
          text-align: right;

          button{
            color: #1BB850;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            i{ color: #000; }
          }
          button:hover{
            background-color: #e8f7ed;
            transition: .2s;
          }
        }
        .nav-item{
          margin: 10px;
          color: #1BB850;
          border-radius: 10px;
          text-align: center;
          cursor: pointer;

          button{
            color: #000;
            width: 100%;
            border-radius: 10px;
            padding: 20px;
          }
        }
        .nav-item:hover{ background-color: #e8f7ed; }
      }
    }


    .scroll-header{
      background-color: #fff;
      box-shadow: 0 2px 2px 0 #eee;
      transition: .6s;
    }
    .scroll-header .nav-group .nav-item button{ color: #000; }
    .scroll-header .mobile-menu-btn-box .v-btn--icon.v-size--default .v-icon{ color: #000; transition: .6s; }


  /* intro */
    .intro{
      background: url('../assets/intro.jpg') no-repeat center top / cover;
      min-height: 100vh;
      color: #fff;

      .bg-grey{
        background-color: rgba($color: #000000, $alpha: .6);
        min-height: 100vh;
        padding: 100px 0;
        display: flex;
        position: relative;

        h1{ letter-spacing: 5px; }
      }
      .text-box{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
      }
    }

  /* about */
    .about{
      .group{
        display: flex;
        justify-content: space-between;
        .text-box{ width: 49%; }
        .img-box{ width: 49%;
          img{
            width: 100%;
          }
        }
      }
      .history{
        margin-top: 80px;
        strong{
          display: inline-block;
          width: 50px;
          margin-right: 20px;
        }
      }
    }

  /* services */
    .services{
      background: url('../assets/services.jpg') no-repeat center center / cover;
      background-attachment: fixed;
      color: #fff;
      .bg-grey{
        background-color: rgba(0, 0, 0, .8);
        .inner-box{ padding-bottom: 20px; }

        h1{ font-weight: bold; }
        hr{ width: 240px; margin: 20px auto 100px; }
        
      }
      .group{
        margin: -10px;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        .con-box{
          width: 30%;
          margin-bottom: 30px;
          padding: 10px;
          display: flex;
          .icon-box{
            width: 50px;
            margin-right: 25px;
            .v-icon{
              font-size: 50px;
              color: #1BB850;
            }
          }
          .j-text{ margin-bottom: 0; }
        }
      }
    }

  /* projects */
    .projects{
      .group{
        margin: 0 -10px 0 -10px;
        display: flex;
        flex-wrap: wrap;

        .card-box{
          width: 33.33333%;
          padding: 0 10px;
          img{
            width: 100%;
            margin-bottom: 30px;
          }
          .text-box{
            margin: 0 10px;
            .j-text{ margin-bottom: 0; }
          }
        }
      }
    }

  /* footer */
    footer{
      background-color: #333;
      color: #fff;
      .f-container{
        padding: 60px 40px;
        .group{
          margin: 0 -10px 0 -10px;
          display: flex;
          flex-wrap: wrap;
        }
        .info-box{
          width: 25%;
          padding: 0 10px;
          .j-title{
            margin-bottom: 10px;
          }
          .j-text{
            margin-bottom: 0;
          }
        }
      }
    }


  /* 반응형 */
  @media (max-width: 768px) {
    .logo-box{ p{ font-size: 32px; } }
    .nav-box{ display: none; }

    .mobile-menu-btn-box{ display: block; }
  }

  @media (max-width: 700px) {
    header{ height: 60px; }
    .h-container{ padding: 0 20px; }
    .logo-box{ p{ font-size: 26px; } }
    .mobile-menu-btn-box{
      .v-btn--icon.v-size--default{
        margin: 10px 0;
        .v-icon{ font-size: 26px; }
      }
    }
    .mobile-nav-box{
      .group{
        .close-item{
          height: 60px;
          padding: 10px 20px;
        }
        .nav-item{ 
          button{ padding: 15px 0; }
        }
      }
    }

    .about{
      .group{
        flex-direction: column;
        max-width: 500px;
        margin: 0 auto;
        .text-box{ width: 100%; }
        .img-box{ width: 100%; text-align: center;
          img{
            max-width: 500px;
            margin-bottom: 40px;
          }
        }
      }
      .group:nth-child(1){
        flex-direction: column-reverse;
        .text-box{ margin-bottom: 40px; }
      }
    }

    .services{
      .bg-grey{
        hr{ width: 200px; margin: 16px auto 60px; }
      }
      .group{
        .con-box{
          width: 50%;
          .icon-box{
            .v-icon{
              font-size: 40px;
            }
          }
        }
      }
    }

    .projects{
      .inner-box{ padding-bottom: 20px; }
      .group{
        .card-box{
          width: 50%;
          margin-bottom: 40px;
          img{ margin-bottom: 15px; }
        }
      }
    }

    footer{
      .f-container{
        padding: 30px 20px 0px;
        .info-box{
          width: 50%;
          margin-bottom: 30px;
        }
      }
    }

  }

  @media (max-width: 500px) {
    .services{
      .group{
        .con-box{ width: 100%; }
      }
    }

    .projects{
      .group{
        .card-box{ width: 100%; }
      }
    }
  }
</style>