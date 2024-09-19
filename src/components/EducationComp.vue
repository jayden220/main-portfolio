<template>
    <div class="main-container">
      <div class="edu-container">
        <h3>Education</h3>  
        <div class="education">
          <div>
            <h1 class="edu-head">Life Choices Academy</h1>
            <p class="edu-date">April - Pressent</p>
            <p class="edu-line"></p>
            <br>
          </div>
          <div>
            <p class="edu-content">I am currently enrolled in a comprehensive coding program that emphasizes software development, web development, and advanced programming languages. This program not only enhances my technical skills but also focuses on my professional and personal development. I am excited to apply my learning to real-world projects and pursue a career in the dynamic field of technology.</p>
          </div>
        </div>
        <div class="education">
          <div class="edu-block">
            <h1 class="edu-head">Northlink College</h1>
            <p class="edu-date">January - December 2023</p>
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
          </div>
        </div>
        <div class="education">
          <div>
            <h1 class="edu-head">HTS Bellville</h1>
            <p class="edu-date">2018 - 2022</p>
            <p class="edu-line"></p>
            <br>
          </div>
          <div>
            <p class="edu-content">I successfully completed my Bachelor's matriculation. Beyond academics, I actively engaged in diverse activities, including competitive chess and Mixed Martial Arts (MMA). These pursuits not only enriched my personal development but also instilled in me valuable skills such as strategic thinking, discipline, and resilience.Additionally, I was a dedicated member of the school's media team, where I honed my communication and creative skills through various projects and responsibilities. My time at Bellville Technical High School not only prepared me academically but also fostered a well-rounded approach to learning and personal growth, laying a solid foundation for my future endeavors.</p>
          </div>
        </div>
      </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
.main-container{
  color: beige;
    /* height: 100vh; */
    background-color: rgb(0, 0, 0);
}
.education{
  display: flex;
  flex-direction: column;
  text-align: left;
  width: 80%;
  margin: 0 auto;
}
.edu-head{
  font-size: 60px;
  margin-top: 2em;

  /* font-family: ; gilda display  */
}
.edu-date{
  font: 100;
  color: #6d7b62;
}
.edu-content{
  font-size: 24px;
  display: block;
}
.edu-line{
  background: linear-gradient(4deg, #ffbc00, #ff0058);
  height: 2.5px;
  -webkit-text-fill-color: transparent;    
  /* padding: 0; */
  /* margin: 5px;   */
}
@media only screen and (max-width: 767px){
  .edu-head{
    font-size: 36px;
  }
  .edu-content{
    font-size: 18px;
  }
  .edu-date{
    font-size: 12px;
  }
}
@media only screen and (max-width: 426px){
  .edu-head{
    font-size: 30px;
  }
  .edu-content{
    font-size: 12px;
  }
  .edu-date{
    font-size: 6px;
  }
}
</style>