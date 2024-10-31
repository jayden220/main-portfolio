<template>
    <div class="main-container">
      <div class="edu-container">
        <h3 class="heading">Education</h3>  
        <div class="education">
          <div class="card">
            <div class="card-inner">
              <div class="card-front">
                <p class="edu-head">Life Choices Academy</p>
                <p class="edu-date">April - Pressent</p>
              </div>
              <div class="card-back">
            <p class="edu-content">I am currently enrolled in a comprehensive coding program that emphasizes software development, web development, and advanced programming languages. This program not only enhances my technical skills but also focuses on my professional and personal development. I am excited to apply my learning to real-world projects and pursue a career in the dynamic field of technology.</p>
              </div>
            </div>
          </div>
        </div>

        <div class="education">
        <div class="card">
          <div class="card-inner">
            <div class="card-front">
            <h1 class="edu-head">Northlink College</h1>
            <p class="edu-date">January - December 2023</p>
            </div>
            <div class="card-back">
              <p class="edu-content">I began my IT journey at Northlink College, earning certifications in Comptia A+, N+, Cisco, and ICDL cybersecurity. These built my skills in hardware, networking, IT operations, and cybersecurity. The hands-on training prepared me for a dynamic IT career, and I’m eager to apply my skills while exploring cloud computing and new technologies.</p>

            </div>
          </div>
        </div>

          <!-- <div class="edu-block"> -->
            <!-- <p class="edu-date">January - December 2023</p>
            <p class="edu-line"></p>
            <br>
          </div>
          <div>
            <p class="edu-content">I began my IT journey at Northlink College, earning Comptia A+, N+, and Cisco and ICDL cybersecurity certifications. These provided a solid foundation in computer hardware, networking, IT operations, and cybersecurity fundamentals. With the A+ certification, I gained skills in hardware/software installation, troubleshooting, and IT support. The N+ certification deepened my understanding of networking, including TCP/IP, routing, and network troubleshooting. Cybersecurity training prepared me to address security challenges in modern IT environments. Northlink College offered hands-on training that enriched my theoretical knowledge, preparing me for a dynamic IT career. I'm ready to apply these skills and continue learning in areas like cloud computing and emerging technologies.</p>
            <ul>
              <li>Comptia A+</li>
              <li>Comptia N+</li>
              <li>Comptia IT Operations Specialist Stackable Certification</li>
              <li>Cisco Cybersecurity</li>
            </ul>
          </div> -->
        </div>

        <div class="education">
              <div class="card">
                <div class="card-inner">
                  <div class="card-front">
                    <p class="edu-head">HTS Bellville</p>
                    <p class="edu-date">2018 - 2022</p>
                  </div>
                  <div class="card-back">
                    <p class="edu-content">I completed my Bachelor's matriculation, actively participating in chess, MMA, and the school's media team. These activities developed my strategic thinking, discipline, resilience, and communication skills. My time at Bellville Technical High School prepared me academically and fostered a well-rounded approach to learning and growth, building a strong foundation for my future.</p>
                  </div>
                </div>
              </div>
        </div>
        <h1>Experience</h1>
        <div class="education">
              <div class="card">
                <div class="card-inner">
                  <div class="card-front">
                    <p class="edu-head">Life Choices Studio</p>
                    <p class="edu-date">September 2024 - Present</p>
                  </div>
                  <div class="card-back">
                    <p class="edu-content">I completed my Bachelor's matriculation, actively participating in chess, MMA, and the school's media team. These activities developed my strategic thinking, discipline, resilience, and communication skills. My time at Bellville Technical High School prepared me academically and fostered a well-rounded approach to learning and growth, building a strong foundation for my future.</p>
                  </div>
                </div>
              </div>
        </div>
    </div>
</div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.main-container{
  height: 390vh;
    background-color: rgb(0, 0, 0);
 

}
.edu-container{
  height: 390vh;
}
.education{
  display: flex;
  flex-direction: column;
  text-align: left;
  width: 80%;
  margin: 10em auto;
}
.heading{
 font-size: 2.5em;
 color: #fff;
  padding-top: 5em;
}
.card {
  width: auto;
  height: 400px;
  perspective: 1500px;
}
.card {
  /* width: 190px; */
  /* height: 254px; */
  display: flex;
  /* align-items: center; */
  /* justify-content: center; */
  gap: 5em;
  /* padding: 0px 15px; */
  background-color: red;
  border-radius: 0px;
  border: none;
  color: white;
  position: relative;
  cursor: pointer;
  /* font-weight: 900; */
  /* transition-duration: .2s; */
  /* background: linear-gradient(0deg, #000, #272727); */
  background: linear-gradient(90deg, #ffbc00, #ff0058);

}

.card:before, .card:after {
  content: '';
  position: absolute;
  left: -2px;
  top: -2px;
  border-radius: 0px;
  background: linear-gradient(90deg, #ffbc00, #ff0058);
  background-size: 400%;
  width: calc(100% + 4px);
  height: calc(100% + 4px);
  z-index: -1;
  animation: steam 3s both infinite;
}

@keyframes steam {
  0% {
    background-position: 0 0;
  }

  50% {
    background-position: 100% 0;
  }

  100% {
    background-position: 0 0;
  }
}



.card-inner {
  width: 100%;
  height: 100%;
  position: relative;
  transform-style: preserve-3d;
  transition: transform 0.999s;
}

.card:hover .card-inner {
  transform: rotateY(180deg);
}

.card-front,
.card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
}

.card-front {
  background-color: #000000;
  color: #fff;
  display: flex;
  flex-direction: column;
  align-items: center;
  border: 1px solid #000000;
  border-radius: 0px;
  justify-content: center;
  transform: rotateY(0deg);
}

.card-back {
  background-color: #000000;
  color: #fff;
  display: flex;
  align-items: center;
  border: 0px solid #000000;
  border-radius: 0px;
  justify-content: center;
  text-align: center;
  /* font-size: 24px; */
  transform: rotateY(180deg);
}
.edu-head{
  font-size: 600px;
  margin-top: 0em;

  /* font-family: ; gilda display  */
}
.edu-date{
  font-size: 600px;
  color: #6af400;
}
.edu-content{
  /* font-size: 24px; */
  /* display: block; */
}
.edu-line{
  background: linear-gradient(4deg, #ffbc00, #ff0058);
  height: 2.5px;
  -webkit-text-fill-color: transparent;    
  /* padding: 0; */
  /* margin: 5px;   */
}
/* For screens larger than 1920px */
@media only screen and (min-width: 1920px) {
  .edu-container {
    height: 550vh;
  }
  .edu-head {
    font-size: 80px;
  }
  .edu-content {
    font-size: 30px;
  }
  .edu-date {
    font-size: 18px;
  }
  .main-container{
  height: 430vh;
    background-color: rgb(197, 164, 164);
 

}
  
}

/* For screens larger than 1440px */
@media only screen and (min-width: 1440px) {
  .edu-container {
    height: 500vh;
  }
  .edu-head {
    font-size: 70px;
  }
  .edu-content {
    font-size: 26px;
  }
  .edu-date {
    font-size: 16px;
  }
  .main-container{
  height: 430vh;
    background-color: rgb(0, 0, 0);
 

}
}

/* For screens larger than 1024px */
@media only screen and (min-width: 1024px) {
  .edu-container {
    height: 450vh;
  }
  .edu-head {
    font-size: 60px;
  }
  .edu-content {
    font-size: 22px;
  }
  .edu-date {
    font-size: 14px;
  }
}

/* For landscape orientation on tablets and mobile devices */
@media only screen and (max-width: 1024px) and (orientation: landscape) {
  .edu-container {
    height: 350vh;
  }
  .edu-head {
    font-size: 40px;
  }
  .edu-content {
    font-size: 18px;
  }
  .edu-date {
    font-size: 12px;
  }
}

/* For portrait orientation on tablets and mobile devices */
@media only screen and (max-width: 1024px) and (orientation: portrait) {
  .edu-container {
    height: 520vh;
  }
  .edu-head {
    font-size: 36px;
  }
  .edu-content {
    font-size: 16px;
  }
  .edu-date {
    font-size: 10px;
  }
  .main-container{
  height: 440vh;
    background-color: rgb(52, 182, 59);
 

}
}
</style>