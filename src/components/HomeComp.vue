<template>
    <section class="hero-section">
      <div class="container">
        <div class="hero-content">
          <div class="image-wrapper">
            <img src="your-profile-image.jpg" alt="Your Profile" class="profile-img" />
          </div>
          <div class="text-content">
            <h1>Hi, I am Jayden.</h1>
            <h2>A creative designer based in Belhar Cape Town</h2>
            <p>
              <!-- I design and code beautifully simple things and I love what I do. Just simple like that! -->
            </p>
            <div class="buttons">
              <button class="project-btn">View my work</button>
              <button class="talk-btn">Let's Talk!</button>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "HeroSection",
  };
  </script>
  
  <style scoped>
  /* General Layout */
  .hero-section {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    background-color: #000000;
    color: #fff;
  }
  
  .container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: 20px;
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .hero-content {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }
  
  .image-wrapper {
    flex: 1;
  }
  
  .text-content {
    flex: 1;
    padding-left: 50px;
  }
  
  .profile-img {
    border-radius: 50%;
    width: 300px;
    height: 300px;
    object-fit: cover;
  }
  
  h1, h2 {
    margin: 0;
    font-weight: 700;
  }
  
  h1 {
    font-size: 2.5rem;
    color: #ffffff;
  }
  
  h2 {
    font-size: 2rem;
    color: #a663ff;
  }
  
  p {
    font-size: 1.2rem;
    line-height: 1.6;
    margin-top: 10px;
  }
  
  .buttons {
    margin-top: 20px;
  }
  
  button {
    padding: 10px 20px;
    font-size: 1rem;
    border-radius: 30px;
    cursor: pointer;
    border: none;
  }
  
  .project-btn {
    background-color: transparent;
    color: #fff;
    border: 1px solid #fff;
    margin-right: 20px;
  }
  
  .talk-btn {
    background-color: #a663ff;
    color: #fff;
  }
  
  .talk-btn:hover, .project-btn:hover {
    opacity: 0.9;
  }
  
  /* Mobile Layout */
  @media (max-width: 768px) {
    .container {
      flex-direction: column;
    }
  
    .hero-content {
      flex-direction: column;
      text-align: center;
    }
  
    .text-content {
      padding-left: 0;
      margin-top: 20px;
    }
  
    h1 {
      font-size: 2rem;
    }
  
    h2 {
      font-size: 1.5rem;
    }
  
    p {
      font-size: 1rem;
    }
  
    .profile-img {
      width: 200px;
      height: 200px;
    }
  
    .buttons {
      display: flex;
      flex-direction: column;
    }
  
    .project-btn {
      margin-bottom: 10px;
    }
  }
  </style>
  