<template>
  <div class="about-container">
      <div class="about">
          <div class="about-content">
              <h1>Who I Am: A Passionate Developer Ready for New Challenges</h1>
              <p>"Distinguished by a fervent passion for music production and an insatiable curiosity for the ever-evolving realm of computer technology, I am a results-driven individual with a proven track record of excellence. Renowned for my unwavering dedication and tireless work ethic, I thrive in collaborative environments where my enthusiasm for both music and technology can flourish. With a keen eye for detail and a knack for problem-solving, I consistently deliver high-quality outcomes while actively contributing to team success. My journey in the field of technology began with rigorous training and certification from Northlink College, where I honed my skills and solidified my foundation. Currently, I am furthering my expertise at Life Choices coding academy, immersing myself in the intricacies of coding and software development. This dual focus on music production and technology not only fuels my professional aspirations but also fosters a holistic approach to innovation and creativity. I am deeply committed to lifelong learning and continuous improvement, constantly seeking opportunities to expand my knowledge and skill set. With a versatile skill set and a passion for excellence, I am poised to make a significant impact in any endeavor I undertake."</p>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.about-container {
  min-height: 100vh; /* Ensures it takes the full viewport height */
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px; /* Adds padding around the content */
  box-sizing: border-box;
  color: white;
  background-color: rgb(0, 0, 0);
}

.about {
  width: 100%;
  max-width: 800px; /* Sets a maximum width for the content */
  margin: 0 auto;
  padding: 20px;
  box-sizing: border-box;
}

.about-content {
  font-size: clamp(14px, 2vw, 24px); /* Responsive font size */
  line-height: 1.6;
  overflow-y: hidden; /* Prevents vertical overflow */
  max-height: 100vh; /* Restricts height to the viewport */
}

@media only screen and (max-width: 775px) {
  .about-content {
      font-size: clamp(12px, 3vw, 18px); /* Adjusts font size for smaller screens */
  }
}

@media only screen and (max-width: 400px) {
  .about-content {
      font-size: clamp(10px, 4vw, 16px); /* Further adjusts font size for very small screens */
  }
}
</style>
