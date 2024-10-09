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
            <div class="card">
  <!-- <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M20 5H4V19L13.2923 9.70649C13.6828 9.31595 14.3159 9.31591 14.7065 9.70641L20 15.0104V5ZM2 3.9934C2 3.44476 2.45531 3 2.9918 3H21.0082C21.556 3 22 3.44495 22 3.9934V20.0066C22 20.5552 21.5447 21 21.0082 21H2.9918C2.44405 21 2 20.5551 2 20.0066V3.9934ZM8 11C6.89543 11 6 10.1046 6 9C6 7.89543 6.89543 7 8 7C9.10457 7 10 7.89543 10 9C10 10.1046 9.10457 11 8 11Z"></path></svg> -->
  <div class="card__content">
    <div class="card__title">
      <h1 class="edu-head">HTS Bellville</h1>
    </div>
    <p class="card__description"></p>
  </div>
</div>
           
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
.card {
  position: relative;
  width: 300px;
  height: 200px;
  background: linear-gradient(-45deg, #f89b29 0%, #ff0f7b 100% );
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
}

.card svg {
  width: 48px;
  fill: #333;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
}

.card:hover {
  transform: rotate(0deg) scale(1.1);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

.card__content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%) rotate(-45deg);
  width: 100%;
  height: 100%;
  padding: 20px;
  box-sizing: border-box;
  background-color: #fff;
  opacity: 0;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
}

.card:hover .card__content {
  transform: translate(-50%, -50%) rotate(0deg);
  opacity: 1;
}

.card__title {
  margin: 0;
  font-size: 24px;
  color: #333;
  font-weight: 700;
}

.card__description {
  margin: 10px 0 0;
  font-size: 14px;
  color: #777;
  line-height: 1.4;
}

.card:hover svg {
  scale: 0;
  transform: rotate(-45deg);
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