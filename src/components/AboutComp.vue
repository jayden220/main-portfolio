<template>
  <div class="about-container">
      <div class="about">
          <div class="about-content">
              <h1>Who I Am</h1>
                <span class="who">A Passionate Developer Ready for New Challenges</span>
              <p>"I’m a tech enthusiast with A+ and N+ certifications from Northlink College, where I built a solid foundation in technology. I’m also a self-taught music producer who loves combining creativity with my passion for technology. I produce music for fun at home as a hobby, and I’m currently interning at Life Choices Studio after completing my training at Life Choices Coding Academy. I thrive on problem-solving, collaborating with teams, and delivering high-quality results, always looking for new ways to innovate and grow in both tech and creative spaces."</p>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.about-container {
  min-height:90vh; /* Ensures it takes the full viewport height */
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px; /* Adds padding around the content */
  box-sizing: border-box;
  color: white;
  /* border: #ff0058 solid 5px; */
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
  max-height: 120vh; /* Restricts height to the viewport */
}
.who{
  background: linear-gradient(90deg, #ffbc00, #ff0058);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 1.5rem;
}
h1 {
  font-size: 2.5rem;
  color: #ffffff;
}

@media only screen and (max-width: 775px) {
  .about-content {
      font-size: clamp(12px, 3vw, 18px); /* Adjusts font size for smaller screens */
  }
}

@media only screen and (max-width: 640px) {
  .about-content {
      font-size: clamp(10px, 4vw, 16px); /* Further adjusts font size for very small screens */
      margin-top: 7em;
  }
}
</style>
