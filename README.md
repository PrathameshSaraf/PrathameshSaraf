


<style>
  @import url("https://fonts.googleapis.com/css2?family=Clicker+Script&family=Poppins:wght@200;300;500;600;700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap");


:root {
  --text-black-900: #000000; /* main heading */
  --text-black-700: #322929; /* sub heading */
  --text-black-500: #000000; /*paragraph */
  --bg-white-900: #ffffff; /* background*/
  --bg-black-100: #777575; /* border*/
  --skin-color: #ff1500;
}

body {
  line-height: 1.5;
  font-size: 16px;
  font-family: "Nunito";
}
* {
  margin: 0;
  padding: 0;
  outline: none;
  text-decoration: none;
  box-sizing: border-box;
}
ul {
  list-style: none;
}
::before,
::after {
  box-sizing: border-box;
}
.section {
  background: var(--bg-white-900);
  min-height: 100vh;
  display: block;
  padding: 0 0px;
  opacity: 1;
}
.main-content {
  padding-left: 1px;
}
.hidden {
  display: none !important;
}
.hidden1 {
  opacity: 0;
  transform: translateY(5rem);
}
.padd-15 {
  padding-left: 15px;
  padding-right: 15px;
}
.container {
  max-width: 1100px;
  width: 100%;
  margin: auto;
}
.section .container {
  padding-top: 40px;
  padding-bottom: 20px;
}
.section-title {
  flex: 0 0 100%;
  max-width: 100%;
  margin-bottom: 60px;
}
.section-title h3 {
  color: var(--text-black-900);
}
.section-title h2 {
  font-size: 40px;
  color: var(--text-black-700);
  font-weight: 700;
  position: relative;
}
.section-title h2::before {
  content: "";
  height: 4px;
  width: 4cm;
  background-color: var(--skin-color);
  position: absolute;
  top: 100%;
  left: 0;
}
.section-title h2::after {
  content: "";
  height: 4px;
  width: 3cm;
  background-color: var(--skin-color);
  position: absolute;
  top: 100%;
  left: 0;
  margin-top: 8px;
}

.row {
  display: flex;
  flex-wrap: wrap;
  margin-left: -15px;
  margin-right: -15px;
  position: relative;
}
.row1 {
  display: flex;
  flex-wrap: wrap;
  margin-left: -15px;
  margin-right: -15px;
  position: absolute;
  width: 100pc;
}
.btn-hover {
  width: 170px;
  font-size: 1.2pc;
  font-weight: 600;
  color: #fff;
  cursor: pointer;
  margin: 20px;
  height: 40px;
  text-align: center;
  border: #34333d solid 1px;
  background-size: 300% 100%;

  border-radius: 30px;
  -moz-transition: all 0.4s ease-in-out;
  -o-transition: all 0.4s ease-in-out;
  -webkit-transition: all 0.4s ease-in-out;
  transition: all 0.4s ease-in-out;
}

.btn-hover:hover {
  background-position: 100% 0;
  -moz-transition: all 0.4s ease-in-out;
  -o-transition: all 0.4s ease-in-out;
  -webkit-transition: all 0.4s ease-in-out;
  transition: all 0.4s ease-in-out;
}

.btn-hover:focus {
  outline: none;
}

.btn-hover.color-1 {
  background-image: linear-gradient(
    to right,
    #ff2a00,
    #ec8c69,
    #ff430a,
    #f70000
  );
  box-shadow: 0 4px 15px 0 rgba(236, 116, 149, 0.75);
}
.shadow-dark {
  box-shadow: 0 0 20px rgba(45, 40, 42, 0.75);
}
/* Aside */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Nunito";
}
.sidebar {
  position: fixed;
  left: 0;
  top: 0;
  height: 100%;
  width: 78px;
  background: #11101d;
  padding: 6px 14px;
  z-index: 99;
  transition: all 0.5s ease;
}
.sidebar.open {
  width: 250px;
}
.sidebar .logo-details {
  height: 60px;
  display: flex;
  align-items: center;
  position: relative;
}
.sidebar .logo-details .icon {
  opacity: 0;
  transition: all 0.5s ease;
}
.sidebar .logo-details .logo_name {
  color: #fff;
  font-size: 20px;
  font-weight: 600;
  opacity: 0;
  transition: all 0.5s ease;
}
.sidebar.open .logo-details .icon,
.sidebar.open .logo-details .logo_name {
  opacity: 1;
}
.sidebar .logo-details #btn {
  position: absolute;
  top: 50%;
  right: 0;
  transform: translateY(-50%);
  font-size: 22px;
  transition: all 0.4s ease;
  font-size: 23px;
  text-align: center;
  cursor: pointer;
  transition: all 0.5s ease;
}
.sidebar.open .logo-details #btn {
  text-align: right;
}
.sidebar i {
  color: #fff;
  height: 60px;
  min-width: 50px;
  font-size: 28px;
  text-align: center;
  line-height: 60px;
}
.sidebar .nav-list {
  margin-top: 20px;
  height: 100%;
}
.sidebar li {
  position: relative;
  margin: 8px 0;
  list-style: none;
}
.sidebar li .tooltip {
  position: absolute;
  top: -20px;
  left: calc(100% + 15px);
  z-index: 3;
  background: #fff;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
  padding: 6px 12px;
  border-radius: 4px;
  font-size: 15px;
  font-weight: 400;
  opacity: 0;
  white-space: nowrap;
  pointer-events: none;
  transition: 0s;
}
.sidebar li:hover .tooltip {
  opacity: 1;
  pointer-events: auto;
  transition: all 0.4s ease;
  top: 50%;
  transform: translateY(-50%);
}
.sidebar.open li .tooltip {
  display: none;
}
.sidebar input {
  font-size: 15px;
  color: #fff;
  font-weight: 400;
  outline: none;
  height: 50px;
  width: 100%;
  width: 50px;
  border: none;
  border-radius: 12px;
  transition: all 0.5s ease;
  background: #1d1b31;
}
.sidebar.open input {
  padding: 0 20px 0 50px;
  width: 100%;
}
.sidebar .bx-search {
  position: absolute;
  top: 50%;
  left: 0;
  transform: translateY(-50%);
  font-size: 22px;
  background: #1d1b31;
  color: #fff;
}
.sidebar.open .bx-search:hover {
  background: #1d1b31;
  color: #fff;
}
.sidebar .bx-search:hover {
  background: #fff;
  color: #11101d;
}
.sidebar li a {
  display: flex;
  height: 100%;
  width: 100%;
  border-radius: 12px;
  align-items: center;
  text-decoration: none;
  transition: all 0.4s ease;
  background: #11101d;
}
.sidebar li a:hover {
  background: #fff;
}
.sidebar li a .links_name {
  color: #fff;
  font-size: 15px;
  font-weight: 400;
  white-space: nowrap;
  opacity: 0;
  pointer-events: none;
  transition: 0.4s;
}
.sidebar.open li a .links_name {
  opacity: 1;
  pointer-events: auto;
}
.sidebar li a:hover .links_name,
.sidebar li a:hover i {
  transition: all 0.5s ease;
  color: #11101d;
}
.sidebar li i {
  height: 50px;
  line-height: 50px;
  font-size: 18px;
  border-radius: 12px;
}
.sidebar li.profile {
  position: fixed;
  height: 60px;
  width: 78px;
  left: 0;
  bottom: -8px;
  padding: 10px 14px;
  background: #1d1b31;
  transition: all 0.5s ease;
  overflow: hidden;
}
.sidebar.open li.profile {
  width: 250px;
}
.sidebar li .profile-details {
  display: flex;
  align-items: center;
  flex-wrap: nowrap;
}
.sidebar li img {
  height: 45px;
  width: 45px;
  object-fit: cover;
  border-radius: 6px;
  margin-right: 10px;
}
.sidebar li.profile .name,
.sidebar li.profile .job {
  font-size: 15px;
  font-weight: 400;
  color: #fff;
  white-space: nowrap;
}
.sidebar li.profile .job {
  font-size: 12px;
}
.sidebar .profile #log_out {
  position: absolute;
  top: 50%;
  right: 0;
  transform: translateY(-50%);
  background: #1d1b31;
  width: 100%;
  height: 60px;
  line-height: 60px;
  border-radius: 0px;
  transition: all 0.5s ease;
}
.sidebar.open .profile #log_out {
  width: 50px;
  background: none;
}
.home-section {
  position: relative;
  background: #efefef;
  min-height: 100vh;
  top: 0;
  left: 78px;
  width: calc(100% - 78px);
  transition: all 0.5s ease;
  z-index: 2;
}
.sidebar.open ~ .home-section {
  left: 250px;
  width: calc(100% - 250px);
}
.home-section .text {
  display: inline-block;
  color: #11101d;
  font-size: 25px;
  font-weight: 500;
  margin: 18px;
}
h3.hello1 span {
  font-family: "clicker Script", cursive;
  font-size: 20px;
  font-weight: 700;
  color: var(--skin-color);
}
span.hello1 {
  font-family: "clicker Script", cursive;
  font-size: 30px;
  font-weight: 700;
  color: var(--skin-color);
}

@media (max-width: 420px) {
  .sidebar li .tooltip {
    display: none;
  }
}
/* Home */

:root {
  --background: #ffffff;
  --primary: #3700b3;
}

.container2 {
  display: flex;
  align-items: center;
}


.container2 > .dynamic-txt {
  color: var(--primary);
  font-size: 22px;
  height: 40px;
  line-height: 50px;
  overflow: hidden;
  margin-left: 0 0 0 15px;
  padding-left: 15px;
}
.container2 > .static-txt {
  color: var(--skin-color);
  font-size: 25px;
  font-weight: 300;
}


.dynamic-txt > li {
  list-style: none;
  font-weight: 400;
  position: relative;
  animation: slide 6s steps(2) infinite;
}
@keyframes slide {
  100% {
    top: -50px;
  }
}
.dynamic-txt li span {
  margin: 5px 0;
  line-height: 40px;
}

.dynamic-txt li span::after {
  position: absolute;
  content: "";
  left: 0;
  height: 100%;
  width: 100%;
  line-height: 50px;
  background: var(--background);
  border-left: 2px solid var(--primary);
  animation: typing 3s steps(10) infinite;
}

@keyframes typing {
  40%,
  60% {
    left: calc(100% + 30px);
  }
  100% {
    left: 0;
  }
}

.home {
  min-height: 100vh;
  display: flex;
  color: var(--text-black-700);
}
.home .home-info {
  flex: 0 0 60%;
  max-width: 60%;
}
h2.hello {
  font-size: 30px;
  margin: 15px 0;
  font-weight: 500;
}
h3.hello span {
  font-family: "clicker Script", cursive;
  font-size: 30px;
  font-weight: 500;
  color: var(--skin-color);
}
h3.my-profession {
  font-size: 30px;
  margin: 15px 0;
}
.typing {
  color: var(--skin-color);
}
.home-info p {
  margin-bottom: 70px;
  font-size: 15px;
  font-weight: 300;
  color: var(--text-black-900);
  text-align: justify;
}
.home .home-img {
  flex: 0 0 40%;
  max-width: 40%;
  text-align: center;
  position: relative;
}
.home-img::after {
  content: "";
  position: absolute;
  width: 80px;
  height: 80px;
  border-bottom: 10px solid var(--skin-color);
  border-right: 10px solid var(--skin-color);
  bottom: 1px;
  right: 80px;
}
.home-img::before {
  content: "";
  height: 80px;
  width: 80px;
  position: absolute;
  border-top: 10px solid var(--skin-color);
  border-left: 10px solid var(--skin-color);
  top: -30px;
  left: 80px;
}
.home .home-img img {
  border-radius: 10px;
  height: 400px;
  margin: auto;
}

/* About Page */
.about .about-content {
  flex: 0 0 100%;
  max-width: 100%;
}
.about .about-content .about-text {
  flex: 0 0 100%;
  max-width: 100%;
}
.about .about-content .about-text h3 {
  font-size: 24px;
  margin-bottom: 15px;
  font-weight: 700;
  color: var(--text-black-900);
}
.about .about-content .about-text h3 span {
  color: var(--skin-color);
}
.about .about-content .about-text p {
  font-size: 16px;
  line-height: 25px;
  color: var(--text-black-900);
  padding-top: 10px;
  text-align: justify;
}
.about .about-content .personal-info {
  flex: 0 0 65%;
  max-width: 65%;
  margin-top: 40px;
}
.about .about-content .personal-info .info-item {
  flex: 0 0 50%;
  max-width: 50%;
}
.about .about-content .personal-info .info-item p {
  font-size: 16px;
  font-weight: 600;
  padding: 10px 0;
  color: var(--text-black-900);
  border-bottom: 1px solid var(--text-black-700);
}
.about .about-content .personal-info .info-item p span {
  font-weight: 400;
  color: var(--text-black-900);
  margin-left: 10px;
  display: inline-block;
}
.about .about-content .personal-info .buttons {
  margin-top: 30px;
}
.about .about-content .skills {
  flex: 0 0 35%;
  max-width: 35%;
  margin-top: 40px;
}
.about .about-content .skills .skill-item {
  flex: 0 0 100%;
  max-width: 100%;
}
.about .about-content .skills .skill-item h5 {
  line-height: 40px;
  font-weight: 600;
  font-size: 16px;

  text-transform: capitalize;
}
.about .about-content .skills .skill-item .progress {
  background-color: #d3d1d1;
  height: 7px;
  border-radius: 4px;
  width: 100%;
  position: relative;
}
.about .about-content .skills .skill-item {
  margin-bottom: 25px;
}
.about .about-content .skills .skill-item .progress .progress-in {
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  border-radius: 4px;
  background-color: var(--skin-color);
}
.about .about-content .skills .skill-item .skill-percent {
  color: #000000;
  right: 40px;
  font-size: 50px;
  font-weight: 100;
}

.about .about-content .education,
.about .about-content .experience {
  flex: 0 0 50%;
  max-width: 50%;
  margin-top: 30px;
}
.about .about-content h3.title {
  font-size: 24px;
  margin-bottom: 30px;
  font-weight: 600;
  color: var(--text-black-900);
}
.about .about-content .timeline-box {
  flex: 0 0 100%;
  width: 100%;
}
.about .about-content .timeline {
  background-color: #fff;
  padding: 30px 15px;
  border: 1px solid ;
  border-radius: 10px;
  width: 100%;
  position: relative;
}

.about .about-content .timeline .timeline-item {
  position: relative;
  padding-left: 30px;
  padding-bottom: 1px;
}
.about .about-content .timeline .timeline-item:last-child {
  padding-bottom: 0;
}
.about .about-content .timeline .timeline-item::before {
  content: "";
  width: 2px;
  position: absolute;
  height: 100%;
  left: 7px;
  top: 0;
  background-color: var(--skin-color);
}
.about .about-content .timeline .circle-dot {
  position: absolute;
  left: 0;
  top: 0;
  height: 15px;
  width: 15px;
  border-radius: 50%;
  background-color: var(--skin-color);
}
.about .about-content .timeline .timeline-date {
  font-weight: 1200;
  font-size: 16px;
  margin-bottom: 12px;
  color: var(--text-black-700);
}
.about .about-content .timeline .timeline-date .fa {
  margin-right: 5px;
}
.about .about-content .timeline .timeline-title {
  font-size: 18px;
  font-weight: 600;
  margin-bottom: 15px;
  text-transform: capitalize;

}
.about .about-content .timeline .timeline-text {
  line-height: 20px;
  font-size: 14px;
  text-align: justify;
  color: #34333d;
}

/*=======SkillSets=========*/
.skill-Set {
  width: 100%;
  background-color: #ffffff;
  color: rgb(2, 2, 2);

  align-items: center;
  text-align: center;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
}
.box {
  width: 3pc;
  text-align: center;
}
.box:hover {
  transform: scale(0.8);
}
.skill-title {
  font-size: 25px;
  padding-top: 20px;
}
.skill-name {
  display: inline-block;
  padding: 5px;

  padding: 20px;
  align-items: center;
  text-align: center;
}

.slider__btn {
  position: absolute;
  top: 50%;
  z-index: 10;
  border: none;
  background: rgba(211, 208, 208, 0.7);
  font-family: "Nunito";
  color: #333;
  border-radius: 50%;
  height: 5.5rem;
  width: 5.5rem;
  font-size: 3.25rem;
  cursor: pointer;
}
.slider {
  max-width: 100rem;
  height: 40rem;
  margin: 0 auto;
  position: relative;

  /* IN THE END */
  overflow: hidden;
}

.slider__btn--left {
  left: 6%;
  transform: translate(-50%, -50%);
}

.slider__btn--right {
  right: 6%;
  transform: translate(50%, -50%);
}

.slide {
  position: absolute;

  width: 100%;
  height: 50rem;

  display: block;
  align-items: center;
  justify-content: center;

  /* THIS creates the animation! */
  transition: transform 1s;
}
.dots {
  position: absolute;
  bottom: 5%;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
}

.dots__dot {
  border: none;
  background-color: #b9b9b9;
  opacity: 0.7;
  height: 1rem;
  width: 1rem;
  border-radius: 50%;
  margin-right: 1.75rem;
  cursor: pointer;
  transition: all 0.5s;

  /* Only necessary when overlying images */
  /* box-shadow: 0 0.6rem 1.5rem rgba(0, 0, 0, 0.7); */
}

.dots__dot:last-child {
  margin: 0;
}

.dots__dot--active {
  /* background-color: #fff; */
  background-color: #888;
  opacity: 1;
}
/*============================My Blog Section=================*/
.blog1 {
  flex: 0 0 100%;
  width: 100%;
  background-color: #ffeef3;
  margin-top: 20px;
  border: solid 2px black;
}
.imgB {
  flex: 0 0 20%;
  width: 20%;
}
.blog-content {
  display: block;
}
.textB {
  flex: 0 0 80%;
  width: 80%;
  padding-bottom: 0px;
}
/*=====================contact page==========================*/
.contact-title {
  color: var(--skin-color);
  text-align: center;
  font-size: 25px;
  margin-bottom: 20px;
}
.contact-sub-title {
  color: var(--text-black-900);
  text-align: center;
  font-size: 15px;
  margin-bottom: 60px;
}
.contact .contact-info-item {
  flex: 0 0 25%;
  width: 25%;
  text-align: center;
  margin-bottom: 60px;
}
.contact .contact-info-item .icon {
  display: inline-block;
}
.contact .contact-info-item .icon .fa {
  font-size: 28px;
  color: var(--skin-color);
}
.contact .contact-info-item h4 {
  font-size: 18px;
  font-weight: 700;

  text-transform: capitalize;
  margin: 15px 0 5px;
}
.contact .contact-info-item p {
  font-size: 16px;
  line-height: 25px;
  color: var(--text-black-700);
  font-weight: 400;
}
.contact .contact-form {
  flex: 0 0 100%;
  min-width: 100%;
}
.contact .contact-form .col-6 {
  flex: 0 0 50%;
  max-width: 50%;
}
.contact .contact-form .col-12 {
  flex: 0 0 100%;
  max-width: 100%;
}
.contact .contact-form .form-item {
  margin-top: 30px;
}
.contact .contact-form .form-item .form-control {
  width: 100%;
  height: 50px;
  border-radius: 25px;

  border: 1px solid var(--text-black-700);
  padding: 10px 25px;
  font-size: 16px;
  color: var(--text-black-700);
  transition: all 0.3s ease;
}
.contact .contact-form .form-item .form-control:focus {
  box-shadow: 0 0 20px rgba(20, 19, 19, 0.5);
}
.contact .contact-form .form-item textarea.form-control {
  height: 140px;
}
/*=================icons=============*/
.social-buttons {
  display: flex;
  flex-wrap: wrap;
  justify-content: left;
  margin-top: -10px;
}

.social-button {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  outline: none;
  width: 50px;
  height: 50px;
  text-decoration: none;
  border-radius: 100%;
  background: #fff;
  text-align: center;
}
.social-button::after {
  content: "";
  position: absolute;
  top: -1px;
  left: 50%;
  display: block;
  width: 0;
  height: 0;
  border-radius: 100%;
  transition: 0.3s;
}
.social-button:focus,
.social-button:hover {
  color: #fff;
}
.social-button:focus::after,
.social-button:hover::after {
  width: calc(100% + 2px);
  height: calc(100% + 2px);
  margin-left: calc(-50% - 1px);
}
.social-button i,
.social-button svg {
  position: relative;
  z-index: 1;
  transition: 0.3s;
}
.social-button i {
  font-size: 28px;
}
.social-button svg {
  height: 40%;
  width: 40%;
}
.social-button--mail {
  color: #0072c6;
}
.social-button--mail::after {
  background: #0072c6;
}
.social-button--facebook {
  color: #3b5999;
}
.social-button--facebook::after {
  background: #3b5999;
}
.social-button--linkedin {
  color: #0077b5;
}
.social-button--linkedin::after {
  background: #0077b5;
}
.social-button--github {
  color: #6e5494;
}
.social-button--github::after {
  background: #6e5494;
}
.social-button--codepen {
  color: #fa0743;
}
.social-button--codepen::after {
  background: #f81335;
}
.social-button--steam {
  color: #7da10e;
}
.social-button--steam::after {
  background: #7da10e;
}
.social-button--snapchat {
  color: #eec900;
}
.social-button--snapchat::after {
  background: #eec900;
}
.social-button--twitter {
  color: #55acee;
}
.social-button--twitter::after {
  background: #55acee;
}
.social-button--instagram {
  color: #e4405f;
}
.social-button--instagram::after {
  background: #e4405f;
}
.social-button--npmjs {
  color: #c12127;
}
.social-button--npmjs::after {
  background: #c12127;
}
@media (max-width: 1199px) {
  .aside {
    left: -270px;
  }
  .main-content {
    padding-left: 0;
  }
  .about .about-content .personal-info.info-item p span {
    display: block;
    margin-left: 0;
  }
  .home-img::before {
    top: -40px;
    left: 40px;
}
.home-img::after {
  bottom: 30px;
    right: 40px;
}

}

@media (max-width: 991px) {
  .contact .contact-info-item,
  .portfolio .portfolio-item,
  .service.service-item
  {
    flex: 0 0 50%;
    max-width: 50%;
  }
  .about .about-content .education, .about .about-content .experience{
    flex: 0 0 100%;
    max-width: 100%;
  }
  .home .home-info {
    flex: 100%;
    max-width: 100%;
  }
  .home .home-img {
    flex: 0 0 100%;
    max-width: 100%;
    text-align: center;
    position: relative;
    padding-bottom: 10px;
}
.home-img::before {
  top: -30px;
  left: 200px;
}
.home-img::after {
bottom: -20px;
  right: 200px;
  padding-bottom: 10px;
}
}

@media (max-width: 767px) {
  .contact .contact-form .col-6,
  .contact .contact-info-item,
  .portfolio .portfolio-item,
  .service.service-item,
  .about .about-content .experience,
  .about .about-content .education,
  .about .about-content .skills,
  .about .about-content .personal-info {
    flex: 0 0 100%;
    max-width: 100%;
  }
  .home-img::before {
    top: -30px;
    left: 120px;
  }
  .portfolios {
    grid-template-columns: repeat(2, 1fr);
  }
  .home-img::after {
  bottom: -15px;
    right: 120px;
    padding-bottom: 10px;
  }
  .skills {
    width: 100%;
    background-color: #ffffff;
    color: rgb(2, 2, 2);
    padding: 30px 30px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
  }
  .social-buttons {
    max-width: 200px;
  }
  .portfolios {
    grid-template-columns: repeat(1, 1fr);
  }
}


.portfolios {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 2rem;
  margin-top: 3rem;
}
.portfolios .portfolio-item {
  position: relative;
  border-radius: 15px;
}
.portfolios .portfolio-item img {
  width: 100%;
  height:150px;
  border: solid 3px black;

  border-radius: 15px;
}
.portfolios .portfolio-item .hover-items {
  width: 100%;
  height: 150px;
  background-color:rgb(213, 213, 213);
  position: absolute;
  left: 0;
  top: 0;
  border-radius: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  opacity: 0;
  transform: scale(0);
  transition: all 0.4s ease-in-out;
}
.portfolios .portfolio-item .hover-items h3 {
  font-size: 1.5rem;

  margin-bottom: 1.5rem;
}
.portfolios .portfolio-item .hover-items .icons {
  display: flex;
  justify-content: center;
  align-items: center;
}
.portfolios .portfolio-item .hover-items .icons .icon {

  border-radius: 50%;
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 1rem;
  cursor: pointer;
  transition: all 0.4s ease-in-out;
}
.portfolios .portfolio-item .hover-items .icons .icon i {
  font-size: 1.5rem;
  color:black;
  margin: 0 1rem;
}
.portfolios .portfolio-item .hover-items .icons .icon:hover {

}
.portfolios .portfolio-item .hover-items .icons .icon:hover i {
  color: black;
}

.portfolio-item:hover .hover-items {
  opacity: 1;
  transform: scale(1);
}

.blogs {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 2rem;
  margin-top: 3rem;
}
.blogs .blog {
  position: relative;

  border-radius: 5px;
  box-shadow: 1px 1px 20px rgba(0, 0, 0, 0.1);
  transition: all 0.4s ease-in-out;
}
.blogs .blog:hover {
  box-shadow: 1px 1px 20px rgba(0, 0, 0, 0.3);
  transform: translateY(-5px);
  transition: all 0.4s ease-in-out;
}
.blogs .blog:hover img {
  filter: grayscale(0);
  transform: scale(1.1);
  box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.8);
}
.blogs .blog img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  filter: grayscale(100%);
  transition: all 0.4s ease-in-out;
}
.blogs .blog .blog-text {
  margin-top: -7px;
  padding: 1.1rem;
  border-top: 8px solid ;
}
.blogs .blog .blog-text h4 {
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 0.7rem;
  transition: all 0.4s ease-in-out;
  cursor: pointer;
}
.blogs .blog .blog-text h4:hover {

}
.blogs .blog .blog-text p {

  font-size: 13px;
  line-height: 1rem;
   text-align: justify;
}

@media screen and (max-width: 600px) {
  .container {
    padding: 1.5rem 2rem !important;
  }
  .portfolios {
    grid-template-columns: repeat(1, 1fr);
    padding-bottom: 6rem;
    margin-top: 1rem;
  }
  .blogs .blog .blog-text h4 {
    font-size: 1.2rem;
  }
  .blogs .blog .blog-text p {
    line-height: 1.5rem;
  }
  .blogs {
    grid-template-columns: repeat(1, 1fr);
    padding-bottom: 6rem;
  }
}
@media screen and (max-width: 1250px) {
  .blogs {
    grid-template-columns: repeat(3, 1fr);
    margin-top: 6rem;
  }

  .portfolios {
    grid-template-columns: repeat(3, 1fr);
  }

 }
@media screen and (max-width: 770px) {
  .portfolios {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media screen and (max-width: 660px) {
  .blogs {
    grid-template-columns: repeat(2, 1fr);
  }

  .portfolios {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media screen and (max-width: 600px) {
  .blogs {
    grid-template-columns: repeat(1, 1fr);
  }

  .portfolios {
    grid-template-columns: repeat(1, 1fr);
    max-width: 70%;
  }
  .portfolios .portfolio-item img{
    width: 70%;
    height: 150px;
  }
  .row .blogs{
    width: 70%;
    max-width: 70%;
  }
  .home-img::before {
    top: -30px;
    left: 90px;
}
.home-img::after {
  bottom: -20px;
  right: 90px;
  padding-bottom: 10px;
}
}
@media (max-width: 570px){
  .home-img::after {
    right: 70px;
    bottom: -20px;
    height: 60px;
    width: 60px;
  }
  .home-img::before {
    left: 50px;
    top: -20px;
    height: 60px;
    width: 60px;
  }
  }
  @media (max-width: 530px){
    .home-img::after {
      right: 30px;
      bottom: -20px;
      height: 60px;
      width: 60px;
    }
    .home-img::before {
      left: 30px;
      top: -30px;
      height: 60px;
      width: 60px;
    }
    }
    @media (max-width: 400px) {
      .social-buttons {
        max-width: 250px;
        padding-left: 20px;
      }
      .social-buttons__button .social-button .social-button--facebook {
        padding-left: 20px;
        padding-right: 20px;
      }
      .portfolios {
        grid-template-columns: repeat(1, 1fr);
        max-width: 100%;
      }
      .portfolios .portfolio-item img{
        width: 100%;
        height: 150px;
      }
      .row .blogs{
        width: 100%;
        max-width: 100%;
      }
      .skill-name {
        width: 70px;
        height: 90px;
        padding-left: 0px;
        padding-top: 0px;
        padding-right: 0px;
        padding-bottom: 0px;
      }
      .home-img::after {
        right: 30px;
        bottom: -10px;
        height: 60px;
        width: 60px;
      }
      .home-img::before {
        left: 70px;
        top: -20px;
        height: 60px;
        width: 60px;
      }
      .btn-hover {
        text-align: center;
        width: 150px;
        font-size: 1pc;
        font-weight: 400;
        color: #fff;
        margin: 10px;
        height: 30px;
        text-align: center;
      }
      .section-title h2 {
        font-size: 30px;
        color: var(--text-black-900);
        font-weight: 500;
      }
      .home .home-img {
        display: inline-block;

        padding-left: 50px;
      }
      .home .home-img img {
        height: 250px;
      }
      .home-img {
        padding-bottom: 80px;
      }
      h2.hello {
        font-size: 25px;
      }
      .home-info p {
        font-size: 13px;
      }
      .container2 > .dynamic-txt {
        font-size: 20px;
        height: 40px;
      }

      .about .about-content .personal-info .row {
        display: inline;
      }
      .about .about-content .personal-info .buttons {
        margin-top: 30px;
        margin-left: 25px;
      }
      .about .about-content .timeline .timeline-title {
        font-size: 16px;
        font-weight: 600;
        margin-bottom: 15px;
        text-transform: capitalize;

      }
      .about .about-content .timeline .timeline-text {
        line-height: 20px;
        font-size: 12px;
      }
      .about .about-content .timeline .timeline-item {
        position: relative;
        padding-left: 27px;
        padding-bottom: 20px;
      }
      .about .about-content .personal-info .info-item {
        flex: 0 0 100%;
        max-width: 100%;
      }
      .sidebar {
        display: none;
      }
      .home,
      .contact .contact-form .col-6,
      .contact .contact-info-item,
      .portfolio .portfolio-item,
      .service.service-item,
      .about .about-content .experience,
      .about .about-content .education,
      .about .about-content .skills,
      .about .about-content .personal-info {
        flex: 0 0 100%;
        max-width: 100%;
      }
      .about .about-content .skill-set {
        max-width: 0;
      }
      .home-section {
        left: 0px;
        width: 350px;
      }
      .personal-info {
        flex: 0 0 20%;
        max-width: 20%;
      }
    }


/* SKILLSET */

.tech {
  width: 100%;
  background-color: #ffffff;
  color: rgb(2, 2, 2);
  padding: 30px 30px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
}

.box:hover {
  transform: scale(0.8);
}

</style>
<section class="home section" id="home">
  <div class="container">
    <div class="row">
      <div class="home-img padd-15">
        <img src="c:\Users\pgsar\Desktop\saraf1.jpg" alt="" />
      </div>
      <div class="home-info padd-15">
          <h2 class="hello">Hello there ! My name is <span class="hello1">  Prathamesh Saraf</span></h2>

          <div class="container2">
            <div class="static-txt"><h3> I'm</h3></div>
            <ul class="dynamic-txt">
              <li><span>Java Developer</span></li>
              <li><span>Web Developer</span></li>


            </ul>

          </div>
          <p>
            I am a Student and studying B-Tech at Vishwakarma Institude of Technology, Pune in electronics and telecommunication fields.
            I graduated with a diploma from the Government Polytechnic, Jalgaon .
          </p>
          <div>

            <div class="social-buttons" style="width: 350px;height: 60px;">
              <a
                href="https://www.facebook.com/prathamesh.saraf.5"
                class="social-buttons__button social-button social-button--facebook"
                aria-label="Facebook"
                target="_blank"
              >
                <i class="fab fa-facebook-f"></i>
              </a>
              <a
                href="https://www.linkedin.com/in/prathamesh-saraf-989663220"
                class="social-buttons__button social-button social-button--linkedin"
                aria-label="LinkedIn" target="_blank"
              >
                <i class="fab fa-linkedin-in"></i>
              </a>
              <a
                href="https://github.com/PrathameshSaraf"
                class="social-buttons__button social-button social-button--github"
                aria-label="GitHub" target="_blank"
              >
                <i class="fab fa-github"></i>
              </a>
              <a
                href="https://instagram.com/prathamesh.saraf_?igshid=YmMyMTA2M2Y="
                class="social-buttons__button social-button social-button--codepen"
                aria-label="CodePen" target="_blank"
              >
                <i class="fab fa-instagram"></i>
              </a>
            </div>

          </div>
         <div style=" padding-top: 80px; padding-left: 10px;">
        <a href="#about">
          <button class="btn-hover color-1">More About Me</button></a
        ></div>
      </div>

    </div>
  </div>
</section>
- 🌱 I’m currently learning **Web-Development** - 👨‍💻 All of my projects are
available at [..](......) - 💬 Ask me abouava And Python** - 📫 How to
reach me **prathameshsaraf2002@gmail.com** - 📄 Know about my experiences
[......](......)

<h3 align="left">Connect with me:</h3>
<p align="left">
  <a href="https://twitter.com/@saraf8624" target="blank"
    ><img
      align="center"
      src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg"
      alt="@saraf8624"
      height="30"
      width="40"
  /></a>
  <a
    href="https://linkedin.com/in/https://www.linkedin.com/in/prathamesh-saraf-989663220"
    target="blank"
    ><img
      align="center"
      src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg"
      alt="https://www.linkedin.com/in/prathamesh-saraf-989663220"
      height="30"
      width="40"
  /></a>
  <a href="https://fb.com/prathamesh saraf" target="blank"
    ><img
      align="center"
      src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg"
      alt="prathamesh saraf"
      height="30"
      width="40"
  /></a>
  <a href="https://instagram.com/prathamesh.saraf" target="blank"
    ><img
      align="center"
      src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg"
      alt="prathamesh.saraf"
      height="30"
      width="40"
  /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left">
  <a href="https://developer.android.com" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original-wordmark.svg"
      alt="android"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer">
    <img
      src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg"
      alt="arduino"
      width="40"
      height="40"
    />
  </a>
  <a href="https://backbonejs.org" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/backbonejs/backbonejs-original-wordmark.svg"
      alt="backbonejs"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg"
      alt="c"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg"
      alt="cplusplus"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg"
      alt="css3"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.djangoproject.com/" target="_blank" rel="noreferrer">
    <img
      src="https://cdn.worldvectorlogo.com/logos/django.svg"
      alt="django"
      width="40"
      height="40"
    />
  </a>
  <a href="https://git-scm.com/" target="_blank" rel="noreferrer">
    <img
      src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg"
      alt="git"
      width="40"
      height="40"
    />
  </a>
  <a href="https://heroku.com" target="_blank" rel="noreferrer">
    <img
      src="https://www.vectorlogo.zone/logos/heroku/heroku-icon.svg"
      alt="heroku"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg"
      alt="html5"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.java.com" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg"
      alt="java"
      width="40"
      height="40"
    />
  </a>
  <a
    href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"
    target="_blank"
    rel="noreferrer"
  >
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg"
      alt="javascript"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.mathworks.com/" target="_blank" rel="noreferrer">
    <img
      src="https://upload.wikimedia.org/wikipedia/commons/2/21/Matlab_Logo.png"
      alt="matlab"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg"
      alt="mongodb"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.mysql.com/" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg"
      alt="mysql"
      width="40"
      height="40"
    />
  </a>
  <a href="https://opencv.org/" target="_blank" rel="noreferrer">
    <img
      src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg"
      alt="opencv"
      width="40"
      height="40"
    />
  </a>
  <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg"
      alt="pandas"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.php.net" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg"
      alt="php"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.postgresql.org" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg"
      alt="postgresql"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.python.org" target="_blank" rel="noreferrer">
    <img
      src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg"
      alt="python"
      width="40"
      height="40"
    />
  </a>
  <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer">
    <img
      src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg"
      alt="scikit_learn"
      width="40"
      height="40"
    />
  </a>
  <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer">
    <img
      src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg"
      alt="seaborn"
      width="40"
      height="40"
    />
  </a>
  <a href="https://spring.io/" target="_blank" rel="noreferrer">
    <img
      src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg"
      alt="spring"
      width="40"
      height="40"
    />
  </a>
  <a href="https://www.tensorflow.org" target="_blank" rel="noreferrer">
    <img
      src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg"
      alt="tensorflow"
      width="40"
      height="40"
    />
  </a>
</p>

<p>
  <img
    align="left"
    src="https://github-readme-stats.vercel.app/api/top-langs?username=prathameshsaraf&show_icons=true&locale=en&layout=compact"
    alt="prathameshsaraf"
  />
</p>

<p>
  &nbsp;<img
    align="center"
    src="https://github-readme-stats.vercel.app/api?username=prathameshsaraf&show_icons=true&locale=en"
    alt="prathameshsaraf"
  />
</p>
