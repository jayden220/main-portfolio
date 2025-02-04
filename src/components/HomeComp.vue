<template>
  <section class="hero-section">
    <div class="container">
      <div class="hero-content">
        
        <div class="image-wrapper">
          <img src="https://jayden220.github.io/hostedImages/images/IMG_9566.png" alt="Your Profile" class="profile-img" loading="lazy"/>
        </div>
        <div class="text-content">
          <h1>Hi, I am Jayden.</h1>
          <h2>A creative designer based in Belhar, Cape Town</h2>
                  <p>
                    Coding, collaborating, and creating—always striving for excellence.
                  </p>
          <div class="buttonsgroup">
            <a class="btn" href="#projects">Explore My Projects</a>
            <a class="btn" href="#contact">Connect with Me</a>
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
.hero-section {
  margin-top: -100px;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: #000000;
  color: #fff;
}

.container {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 4em;
  padding: 20px;
  max-width: 1200px;
  width: 100%;
}

.hero-content {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}

.image-wrapper {
  flex: 1.5;
  text-align: center; /* Center image in small screens */
}




.text-content {
  flex: 1;
}

.profile-img {
  width: 100%; /* Make the image responsive */
  max-width: 200px; /* Maintain max size */
  margin-top: 4.5em;
  height: auto; /* Maintain aspect ratio */
  border: 2px solid transparent; /* Set border to transparent */
  border-image:linear-gradient(4deg, #ffbc00, #ff0058) 1; /* Add gradient border */
  
  transition: transform 0.3s ease;
}
.profile-img:hover {
  transform: scale(1.01);
  box-shadow: 0px 3px 8px   #ffbc00; /* Add glow effect */
}
h1, h2 {
  margin: 0;
  font-weight: 500;
}

h1 {
  font-size: 2.5rem;
  color: #ffffff;
}

h2 {
  font-size: 2rem;
  background: linear-gradient(90deg, #ffbc00, #ff0058) ;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

p {
  font-size: 1.2rem;
  line-height: 1.6;
  margin-top: 10px;
}

.buttonsgroup {
  margin-top: 20px;
  display: flex;
  gap: 1em;
  justify-content: center; /* Center buttons */
  flex-wrap: wrap; /* Wrap buttons on small screens */

}
.btn {
 display: inline-block;
 padding: 0.9rem 1.8rem;
 font-size: 17px;
 font-weight: 200;
 color: white;
 border: .1px solid rgb(255, 255, 255);
 cursor: pointer;
 position: relative;
 background-color: transparent;
 text-decoration: none;
 overflow: hidden;
 z-index: 1;
 font-family: inherit;
 border-radius: 0px;
}

.btn::before {
 content: "";
 position: absolute;
 left: 0;
 top: 0;
 width: 100%;
 height: 100%;
 border-radius: 0px;
background: linear-gradient(40deg, #ffbc00, #ff0058);
 transform: translateX(-100%);
 transition: all .3s;
 z-index: -1;
}

.btn:hover::before {
 transform: translateX(0);
 border-radius: 0px;
 border: none;
}



.project-btn {
  background-color: transparent;
  margin-right: 1em;
}

.talk-btn {
  border: none;
}

@media (max-width: 900px) {
  .container {
    flex-direction: column;
    /* padding: 10px; */
  }

  .hero-content {
    flex-direction: column;
    text-align: center;
  }

  .text-content {
    margin-top: 2em;
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
    width: 80%; /* More responsive on small screens */
    max-width: 300px;
    margin-top: 6em;
  }

  .buttons {
    flex-direction: column;
    align-items: center;
    /* margin: 0 2em; */
  }

  /* .project-btn {
    margin-bottom: 10px;
    margin-right: 0;
    border-radius: 25px ;
  } */
}
@media (min-width: 1500px) {
  .hero-section {
    min-height: 80vh; /* Reduce the height to make it more proportional */
  }

  .container {
    max-width: 1400px; /* Increase the max-width to make the content more prominent */
  }

  /* .hero-content {
  transform: scale(1.2); 
} */

  .text-content {
    font-size: 1.5rem; /* Increase the font size to make it more readable */
  }

  h1 {
    font-size: 3.5rem; /* Increase the font size of the heading */
  }

  h2 {
    font-size: 2.5rem; /* Increase the font size of the subheading */
  }

  .profile-img {
    max-width: 400px; /* Increase the max-width of the profile image */
  }
}

/* Additional media queries for smaller screens */
@media (max-width: 768px) {
  h1 {
    font-size: 2rem;
  }
  h2 {
    font-size: 1.7rem;
  }
  .btn {
    font-size: 1rem;
  }

  .profile-img {
    width: 100%; /* Even smaller for very small screens */
    max-width: 200px;
    margin-top: 5em;
  }
}

/* For very small screens */
@media (max-width: 640px) {
  h1 {
    font-size: 1.5rem;
  }

  h2 {
    font-size: 1.2rem;
  }

  p {
    font-size: 0.8rem;
  }
  .profile-img {
    width: 100%; /* Even smaller for very small screens */
    max-width: 200px;
    margin-top: 10em;
  }
}
</style>
