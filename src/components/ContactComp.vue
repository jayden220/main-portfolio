<template>
    <section id="contact">
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
            <p>jaydenvanrooyen87@@mail.com</p>
            <p></p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');
  
  #contact {
    background-color: #000000;
    color: #fff;
    padding: 50px 20px;
    font-family: 'Roboto', sans-serif;
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
  
  .contact-info {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    font-size: 1.1rem;
  }
  
  h2 {
    font-size: 2rem;
    margin-bottom: 10px;
    color: #fff;
  }
  
  .highlight {
    background: linear-gradient(4deg, #ffbc00, #ff0058);
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
  
  button {
    width: 100%;
    padding: 12px;

    border: none;
    color: #fff;
    font-size: 1rem;
    cursor: pointer;
    /* border-radius: 5px; */
    transition: background-color 0.3s;
  }
  
  button:hover {
    background-color: linear-gradient(4deg, #ffbc00, #ff0058);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
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
  
  