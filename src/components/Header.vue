<template>
  <header>
    <div class="header-wrapper">
      <div class="video-intro">
        <video
          src="../img/dev1.mp4"
          class="video-intro-wraper__video"
          muted
          autoplay
          loop
          preload="auto"
        ></video>
        <nav class="header-nav">
          <input type="checkbox" id="menu" />
          <label for="menu" class="menu__btn">
            <span></span>
          </label>
          <ul class="header-nav-menu" id="slow">
            <li>
              <a href="#about" class="header-nav-menu__item">ABOUT ME</a>
            </li>
            <li>
              <a href="#exp" class="header-nav-menu__item">EXPERIENCE</a>
            </li>
            <li>
              <a href="#skills" class="header-nav-menu__item">SKILLS</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header-nav {
  visibility: hidden;
}
.video-intro-wraper__video {
  position: fixed;
  opacity: 20%;
  width: 100%;
  z-index: -1;
}
.header-nav-menu {
  justify-content: space-around;
  display: flex;
  list-style: none;
  width: 50%;
  padding-right: 30px;
  margin: 0 0 0 auto;
  font-family: 'Lato Bold';
  color: #504f4f;
  height: 10px;
}
.header-nav-menu a {
  text-decoration: none;
  color: rgb(85, 83, 83);
  font-size: 25px;
}
#menu {
  opacity: 0;
}
@media screen and (max-width: 992px) {
  .header-nav {
    visibility: visible;
  }
  #menu {
    opacity: 0;
  }
  .menu__btn {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    position: fixed;
    top: 10px;
    right: 2%;
    width: 30px;
    height: 30px;
    cursor: pointer;
    z-index: 2;
  }
  .menu__btn span,
  .menu__btn span:before,
  .menu__btn span:after {
    position: absolute;
    display: block;
    width: 100%;
    height: 3px;
    background-color: rgb(80, 79, 79);
    -webkit-transition: 0.4s;
    -o-transition: 0.4s;
    transition: 0.4s;
  }
  .menu__btn span:before {
    content: '';
    top: -10px;
  }
  .menu__btn span:after {
    content: '';
    top: 10px;
  }
  .header-nav-menu {
    position: fixed;
    visibility: hidden;
    top: 0;
    right: -100%;
    width: 40%;
    height: -webkit-fit-content;
    height: -moz-fit-content;
    height: fit-content;
    padding-left: 0;
    text-align: center;
    background-color: #3c3c3c;
    -webkit-transition: 0.4s;
    -o-transition: 0.4s;
    -webkit-transition: 0.6s;
    -o-transition: 0.6s;
    transition: 0.6s;
    opacity: 0.97;
    border-radius: 5px;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
  }
  .header-nav-menu__item {
    text-decoration: none;
    padding: 5px 5px;
    display: block;
    text-transform: uppercase;
    font-size: 16px;
    font-family: sans-serif;
    color: #fff;
    -webkit-transition: 0.3s;
    -o-transition: 0.3s;
    transition: 0.3s;
  }
  .header-nav-menu__item li:hover {
    cursor: pointer;
  }
  .header-nav-menu__item:checked,
  .header-nav-menu__item:hover {
    cursor: pointer;
    color: rgb(126, 126, 141);
    text-decoration: none;
  }
  #menu:checked ~ .header-nav-menu {
    visibility: visible;
    right: 0;
    z-index: 1;
  }
  #menu:checked ~ .menu__btn span {
    -webkit-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    transform: rotate(45deg);
    background-color: #fff;
  }
  #menu:checked ~ .menu__btn span:before {
    -webkit-transform: rotate(0);
    -ms-transform: rotate(0);
    transform: rotate(0);
    top: 0;
    background-color: #fff;
  }
  #menu:checked ~ .menu__btn span:after {
    -webkit-transform: rotate(90deg);
    -ms-transform: rotate(90deg);
    transform: rotate(90deg);
    top: 0;
    background-color: #fff;
  }
}
.item-wraper {
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
}
.item-wraper ul:last-child {
  border: none;
  margin-top: 20px;
}
</style>
