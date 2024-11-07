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
  
  <!-- <div class="img"></div> -->
  <h2>Contact <span class="highlight">Info</span> </h2>
      <p class="info">I'm currently available to take on new projects, so feel free to send me a message about anything that you want to run past me. You can contact anytime at 24/7.</p>
        <div class="contact-details">
                <p>+27 78 291 980</p>
                <p>jaydenvanrooyen87@gmail.com</p>
                <p></p>
        </div>
  <button>Resume</button>



        </div>

      </div>
    </section>
  </template>
  
  <style scoped>


  
  #contact {
    background-color: #000000;
    color: #fff;
    padding: 50px 20px;
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
  
  