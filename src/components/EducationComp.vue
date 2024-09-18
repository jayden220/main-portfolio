<template>
    <div class="main-container">
      <div class="edu-container">
        <h3>Education</h3>  
        <div class="education">
          <div>
            <p class="edu-date"> April 2024 - Present</p>
            <h1 class="edu-head">Life Choices</h1>
          </div>
          <div>
            <p class="edu-content">I am currently enrolled in a comprehensive coding program that emphasizes software development, web development, and advanced programming languages. This program not only enhances my technical skills but also focuses on my professional and personal development. I am excited to apply my learning to real-world projects and pursue a career in the dynamic field of technology.</p>
          </div>
        </div>
        <div class="education">
          <div>
            <p class="edu-date"> April 2024 - Present</p>
            <h1 class="edu-head">Northlink</h1>
          </div>
          <div>
            <p class="edu-content">I am currently enrolled in a comprehensive coding program that emphasizes software development, web development, and advanced programming languages. This program not only enhances my technical skills but also focuses on my professional and personal development. I am excited to apply my learning to real-world projects and pursue a career in the dynamic field of technology.</p>
          </div>
        </div>
        <div class="education">
          <div>
            <p class="edu-date"> April 2024 - Present</p>
            <h1 class="edu-head">HTS Bellville</h1>
          </div>
          <div>
            <p class="edu-content">I am currently enrolled in a comprehensive coding program that emphasizes software development, web development, and advanced programming languages. This program not only enhances my technical skills but also focuses on my professional and personal development. I am excited to apply my learning to real-world projects and pursue a career in the dynamic field of technology.</p>
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
  /* font-family: ; gilda display  */
}
.edu-content{
  font-size: 24px;
  display: block;
}
.edu-date{
  font-family: 'InterVariable', sans-serif;
  font-size: 14px;
  color: #cccccc; 
  margin-bottom: 10px;
}
</style>