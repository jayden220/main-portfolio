<template>
  <section class="hero-section">
    <div class="container">
      <div class="hero-content">
        <div class="image-wrapper">
          <img src="your-profile-image.jpg" alt="Your Profile" class="profile-img" />
        </div>
        <div class="text-content">
          <h1>Hi, I am Jayden.</h1>
          <h2>A creative designer based in Belhar, Cape Town</h2>
          <p>
            I design and code beautifully simple things and I love what I do. Just simple like that!
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
.hero-section {
  margin-top: -20px;
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
  gap: 5em;
  padding: 20px;
  max-width: 1200px;
  width: 100%;
}

.hero-content {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}

.image-wrapper {
  flex: 1;
  text-align: center; /* Center image in small screens */
}

.text-content {
  flex: 1;
}

.profile-img {
  border-radius: 50%;
  width: 100%; /* Make the image responsive */
  max-width: 300px; /* Maintain max size */
  height: auto; /* Maintain aspect ratio */
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
  background: linear-gradient(4deg, #ffbc00, #ff0058);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

p {
  font-size: 1.2rem;
  line-height: 1.6;
  margin-top: 10px;
}

.buttons {
  margin-top: 20px;
  display: flex;
  justify-content: center; /* Center buttons */
  flex-wrap: wrap; /* Wrap buttons on small screens */
}

button {
  --border-radius: 15px;
  --border-width: 4px;
  appearance: none;
  position: relative;
  padding: 1em 2em;
  border: 0;
  border-radius: 20px;
  background-color: #000000;
  font-family: "Roboto", Arial, "Segoe UI", sans-serif;
  font-size: 18px;
  font-weight: 500;
  color: #fff;
  z-index: 2;
  cursor: pointer;
  transition: opacity 0.3s ease;
}

button::after {
  --m-i: linear-gradient(#000, #000);
  --m-o: content-box, padding-box;
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  padding: var(--border-width);
  background: linear-gradient(45deg, #ffbc00, #ff0058);
  -webkit-mask-image: var(--m-i), var(--m-i);
  mask-image: var(--m-i), var(--m-i);
  -webkit-mask-origin: var(--m-o);
  mask-origin: var(--m-o);
  -webkit-mask-clip: var(--m-o);
  mask-composite: exclude;
  -webkit-mask-composite: destination-out;
  filter: hue-rotate(0);
  animation: rotate-hue linear 500ms infinite;
  animation-play-state: paused;
}

button:hover::after {
  animation-play-state: running;
}

@keyframes rotate-hue {
  to {
    filter: hue-rotate(1turn);
  }
}

.project-btn {
  background-color: transparent;
}

.talk-btn {
  border: none;
}

@media (max-width: 900px) {
  .container {
    flex-direction: column;
    padding: 10px;
  }

  .hero-content {
    flex-direction: column;
    text-align: center;
  }

  .text-content {
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
    width: 80%; /* More responsive on small screens */
    max-width: 200px;
  }

  .buttons {
    flex-direction: column;
    align-items: center; /* Center buttons vertically */
  }

  .project-btn {
    margin-bottom: 10px;
  }
}

/* Additional media queries for smaller screens */
@media (max-width: 768px) {
  h1 {
    font-size: 1.8rem;
  }

  h2 {
    font-size: 1.4rem;
  }

  p {
    font-size: 0.9rem;
  }

  .profile-img {
    width: 70%; /* Even smaller for very small screens */
    max-width: 180px;
  }
}

/* For very small screens */
@media (max-width: 300px) {
  h1 {
    font-size: 1.5rem;
  }

  h2 {
    font-size: 1.2rem;
  }

  p {
    font-size: 0.8rem;
  }
}
</style>
