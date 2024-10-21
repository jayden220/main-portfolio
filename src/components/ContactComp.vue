<template>
    <section id="contact">
      <h1 class="heading">Contact Me</h1>
      <div class="contact-wrapper">
        <div class="contact-form">
          <h2>Let’s work <span class="highlight">together!</span></h2>
          <p class="contact-description">
            I design and code beautifully simple things and I love what I do. Just simple like that!
          </p>
          
          <form>
            <div class="form-group">
              <input type="text" placeholder="First name" required />
            </div>
            <div class="form-group">
              <input type="text" placeholder="Last name" required />
            </div>
            <div class="form-group">
              <input type="email" placeholder="Email address" required />
            </div>
            <div class="form-group">
              <input type="text" placeholder="Phone number" required />
            </div>
            <button type="submit">Submit</button>
          </form>
        </div>
        <div class="contact-info">
          <p>
            I'm currently available to take on new projects, so feel free to send me a message about
            anything that you want to run past me. You can contact anytime at 24/7.
          </p>
          <div class="contact-details">
            <p>+27 78 291 980</p>
            <p>jaydenvanrooyen87@gmail.com</p>
            <p></p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <style scoped>
@import url('https://fonts.googleapis.com/css2?family=Gilda+Display&display=swap');

  
  #contact {
    background-color: #000000;
    color: #fff;
    padding: 50px 20px;
    font-family: 'Gilda Display', sans-serif;
  }
  
  .contact-wrapper {
    display: flex;
    max-width: 1200px;
    margin: 0 auto;
    gap: 30px;
  }
  
  .contact-form {
    flex: 1;
  }
  .heading{
    margin: 2em 0 ;
  }
  
  .contact-info {
    flex: 1;
    display: flex;
    flex-direction: column;
    /* justify-content: space-between; */
    font-size: 1.1rem;
  }
  
  h2 {
    font-size: 2rem;
    margin-bottom: 10px;
    color: #fff;
  }
  /* From Uiverse.io by mrhyddenn */ 
button {
  position: relative;
  margin: 2em 2em;
  padding: 10px 20px;
  /* border-radius: 7px; */
  border: 1px solid rgb(255, 255, 255);
  font-size: 14px;
  text-transform: uppercase;
  font-weight: 600;
  letter-spacing: 2px;
  background: transparent;
  color: #fff;
  overflow: hidden;
  /* box-shadow: 0 0 0 0 transparent; */
  -webkit-transition: all 0.2s ease-in;
  -moz-transition: all 0.2s ease-in;
  transition: all 1s ease-in;
}

button:hover {
  background: linear-gradient(90deg, #ffbc00, #ff0058);
  /* box-shadow: 0 0 30px 5px  #ffbb0037; */
  -webkit-transition: all 0.2s ease-out;
  -moz-transition: all 0.2s ease-out;
  transition: all 0.2s ease-out;
}

button:hover::before {
  -webkit-animation: sh02 0.5s 0s linear;
  -moz-animation: sh02 0.5s 0s linear;
  animation: sh02 0.5s 0s linear;
}

button::before {
  content: '';
  display: block;
  width: 0px;
  height: 86%;
  position: absolute;
  top: 7%;
  left: 0%;
  opacity: 0;
  background: #fff;
  box-shadow: 0 0 50px 30px #f86336;
  -webkit-transform: skewX(-20deg);
  -moz-transform: skewX(-20deg);
  -ms-transform: skewX(-20deg);
  -o-transform: skewX(-20deg);
  transform: skewX(-20deg);
}

@keyframes sh02 {
  from {
    opacity: 0;
    left: 0%;
  }

  50% {
    opacity: 1;
  }

  to {
    opacity: 0;
    left: 100%;
  }
}

button:active {
  box-shadow: 0 0 0 0 transparent;
  -webkit-transition: box-shadow 0.2s ease-in;
  -moz-transition: box-shadow 0.2s ease-in;
  transition: box-shadow 0.2s ease-in;
}


  .highlight {
    background: linear-gradient(90deg, #ffbc00, #ff0058);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  }
  
  .contact-description {
    font-size: 1.1rem;
    margin-bottom: 20px;
    color: #ccc;
  }
  
  .form-group {
    margin-bottom: 15px;
  }
  
  input {
    width: 100%;
    border: none;
    border-bottom: 1px solid #444;
    background: transparent;
    padding: 8px 0;
    color: #ddd;
    font-size: 1rem;
    outline: none;
  }
  
  input::placeholder {
    color: #888;
  }
  

  
  .contact-info p {
    margin-bottom: 70px;
  }
  
  @media (max-width: 768px) {
    .contact-wrapper {
      flex-direction: column;
    }
  }
  @media (max-width: 1441px) {
    /* .contact-info{
      /* font-size: 350px; */
  
    .contact-info p {
    margin-bottom: 70px;
    /* font-size: 350px; */

  }
  }
  
  </style>
  
  