<template>
  <main>
    <div class="main-wrpper">
      <div class="main-face">
        <img
          src="../img/main_Roman Czujko.png"
          alt="RomanCzujko"
          class="main-face__img--ava"
        />
        <h1 class="main-face__title" id="about">Roman Czujko</h1>
        <p class="main-face__after-title">Front-End Developer</p>
        <p>tel: +38 066 648 9928</p>
        <p>Viber/Watsapp: +38 063 383 1273</p>
        <p>email: roman.czujko@gmail.com</p>
        <a href="https://www.linkedin.com/in/roman-czujko-5411221a2/"
          ><img
            class="main-face__img--social"
            src="../img/Linkedin-Logo.png"
            alt=""
        /></a>
        <div class="main-face__icons">
          <img src="../img/html-5.png" alt="" />
          <img src="../img/css.png" alt="" />
          <img src="../img/sass.png" alt="" />
          <img src="../img/iconfinder_187_Js_logo_logos_4373213.png" alt="" />
          <img src="../img/694px-Vue.js_Logo_2.png" alt="" />
        </div>
      </div>
      <div class="container">
        <div class="row">
          <section class="col-md-12 about about-hidden">
            <h3 class="item-title">AboutMe</h3>
            <div class="item-text">
              <p align="center" class="item-title">
                Hello world! My name is Roman. I'm Front-End Developer.
              </p>
              <img
                src="../img/Developer.png"
                alt="dev"
                class="about-icon-img"
              />
              <p>
                I like to create - Modern websites | Responsive User Interfaces
                | Applications to Business processes for online sales or any
                directions of user interactions with the programs. Improve and
                supporting CMS for online stores OpenCart / Magento /
                Woocommerce.
              </p>
              <p>
                My motto is: self-development and self-improvement. I use new
                and existing technologies. I like to study, sport and good
                music.
              </p>
              <p>
                👨‍💻 I'm working with: HTML5 - CSS3/Sass - Bootstrap/Flex/BEM -
                JS/JQuery/Ajax/API - Git/Gulp/Webpack 👨‍💻
              </p>
            </div>
          </section>
          <section class="col-md-12 experience experience-hidden" id="exp">
            <h3 class="item-title">Experience</h3>
            <ul class="item-text">
              <li>
                2007-2013 > Commercial Bank - eCommerce - Project Manager
                Internet Bankig Project
              </li>
              <li>2012 > IT Courses - Front-End (html/css/js)</li>
              <li>2013-2017 > Manager Charity Project IT direction</li>
              <li>2017 > IT Courses - SEO / GAds / FaceBook Ads</li>
              <li>2020 > IT Courses - Front-End (html/css/js/VUE)</li>
              <li>
                2017 - today > Front-End Developer (+less IT Manager
                Online-Sales) Bernardo Ukraine
              </li>
            </ul>
          </section>
          <section class="col-md-6 skill skill-hidden" id="skills">
            <h3 class="item-title">Skills</h3>
            <div class="item-wraper">
              <ul class="item-text--skills">
                <p class="item-text-list__skills">Hard Skills</p>
                <li>HTML - 85%</li>
                <li>CSS/SCSS - 80%</li>
                <li>JS - 50%</li>
                <li>Vue - 20%</li>
              </ul>
              <ul class="item-text--skills">
                <p class="item-text-list__skills">Soft Skills</p>
                <li>Conscientious</li>
                <li>Cooperative</li>
                <li>Creative</li>
                <li>Eager to learn</li>
                <li>Diligent</li>
              </ul>
            </div>
          </section>
          <section class="col-md-6 add-skills add-skills-hidden">
            <h3 class="item-title">Additional Knowleges</h3>
            <ul class="item-text">
              <li>Bootstrap</li>
              <li>BEM</li>
              <li>Git</li>
              <li>Gulp</li>
              <li>Webpack</li>
              <li>Ajax</li>
              <li>MySQL - basic</li>
              <li>PHP - basic</li>
              <li>Adobe: Photoshop + PrimerPro</li>
              <li>Google: SEO | GAds | GAnalytics | GMaps API</li>
              <li>English - B1/B2 | Polish - B2/C1</li>
            </ul>
          </section>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-face {
  color: #504f4f;
  display: flex;
  flex-direction: column;
  font-size: 14px;
  font-family: 'Lato Bold';
  text-align: center;
  margin-right: 1%;
}
.main-face__title {
  font-size: 40px;
}
.main-face__after-title {
  font-size: 20px;
}
.main-face__img--ava {
  border-radius: 50px;
  width: 150px;
  margin-left: 20px;
  align-self: center;
}
.main-face__img--social {
  height: 40px;
  align-self: center;
}
.main-face__icons {
  display: flex;
  justify-content: center;
  flex-direction: row;
  width: 100%;
  margin-top: 10px;
}
.main-face__icons img {
  height: 50px;
  margin: 0 auto;
}

.main-wrpper {
  display: flex;
  justify-content: space-between;
  margin: 5px 0 0 3%;
  max-width: 1300px;
  margin: 0 auto;
}

.container {
  margin-left: 0;
  margin-right: 0;
}
.row {
  width: 100%;
}

.about {
  animation-name: moveBlock1;
  animation-duration: 1s;
  color: #5a5858;
  transition: all 1s linear;
  animation-timing-function: linear;
  padding: 5px;
  width: 90%;
}

.about-icon-img {
  width: 50px;
  text-align: center;
  float: left;
  margin-right: 10px;
}

.experience {
  animation-name: moveBlock2;
  animation-duration: 2s;
  color: #5a5858;
  transition: all 1s linear;
  animation-timing-function: linear;
  padding: 5px;
  width: 90%;
}

.skill {
  animation-name: moveBlock3;
  animation-duration: 3.5s;
  color: #5a5858;
  transition: all 1s linear;
  animation-timing-function: linear;
  padding: 5px;
  width: 90%;
}

.add-skills {
  animation-name: moveBlock4;
  animation-duration: 4s;
  color: #5a5858;
  transition: all 1s linear;
  animation-timing-function: linear;
  padding: 5px;
  width: 90%;
}

.about-hidden,
.experience-hidden {
  transition: all 1s linear;
}

.skill,
.add-skills {
  color: #5a5858;
  transition: 4s;
}

.skill-hidden,
.add-skills-hidden,
.soft-scills-hidden {
  transition: 4s;
}

.about:hover,
.experience:hover,
.skill:hover,
.add-skills:hover {
  transform: scale(1.02, 1.02);
  transition: 2s;
}

.about::not(:hover),
.experience::not(:hover),
.skill::not(:hover),
.add-skills::not(:hover) {
  transform: scale(1, 1);
  transition: 2s;
}

.item-title {
  text-align: center;
  font-size: 26px;
  margin-bottom: 20px;
}

.item-wraper {
  display: flex;
  justify-content: center;
  box-shadow: 0 0 10px #5a5858;
  border-radius: 20px;
  min-height: 250px;
  padding: 40px 20px 40px 10px;
}

.item-wraper ul:last-child {
  border-left: 2px solid #a09a9a;
}

.item-text {
  font-size: 15px;
  width: 100%;
  padding: 20px 20px 20px 40px;
  box-shadow: 0 0 10px #5a5858;
  border-radius: 20px;
  list-style-position: inside;
}

.item-text--skills {
  margin-right: 20px;
  margin-bottom: 0;
  line-height: 1.6;
  height: 90%;
  font-size: 17px;
}

.item-text-list__skills {
  font-size: 18px;
  font-family: 'Lato Bold';
}
@keyframes moveBlock1 {
  0% {
    transform: translateY(-100%);
  }
  100% {
    transform: translateY(0px);
  }
}
@keyframes moveBlock2 {
  0% {
    transform: translateX(2000px);
  }
  100% {
    transform: translateX(0px);
  }
}
@keyframes moveBlock3 {
  0% {
    transform: translateY(1000px);
  }
  100% {
    transform: translateY(0px);
  }
}
@keyframes moveBlock4 {
  0% {
    transform: translateX(2000px);
  }
  100% {
    transform: translateX(0px);
  }
}
</style>
