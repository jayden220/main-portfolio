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
            <button type="submit" class="btn">Submit</button>
          </form>
        </div>

        <div class="contact-info">
  

  <h2>Contact <span class="highlight">Info</span> </h2>

      
        <div class="contact-details">
          <div class="contact-grid">
            <div class="btn1">
              <h5 >Call Me</h5>
              <p>+27 78 291 980</p>
            </div>
            <div class="btn2">
              <h5>Location</h5>
              <p>South Africa</p>
            </div>
            <div class="btn3">
              <h5>Email</h5>
              <p>jaydenvanrooyen87@gmail.com</p>
            </div>

                
              </div>
        </div>



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
    gap: 5em;
    flex-wrap: wrap;
  }
  
  .contact-form,
  .contact-info{
    flex: 1.9;
    min-width: 300px;
  }
  .heading{
    margin: 2em 0 ;
    text-align: center;
    font-size: 2.5rem;
  }
  .contact-form h2,
.contact-info h2 {
  margin-bottom: 20px;
}
  
.contact-info {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  font-size: 1.1rem;
}y



  .highlight {
    background: linear-gradient(90deg, #ffbc00, #ff0058);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  }
  
  .contact-description {
    font-size: 1rem;
    margin-bottom: 20px;
    color: #ccc;
  }
  
  .form-group {
    margin-bottom: 15px;
    display: flex;
    flex-direction: column;
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
  .contact-details h5 {
  margin: 10px 0;
  font-size: 1rem;
 
}

.contact-details p {
  margin: 5px 0;
  color: #ddd;
  display: inline;
}
.contact-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(10px, 2fr)); /* Default layout */
  gap: 10px;
}

.contact-grid div {
    /* background: linear-gradient(90deg, #ffbc00, #ff0058); */
    /* background: #504747; */
  padding: 10px;
  border-radius: 0px;
  text-align: center;
}
.contact-grid .mail {
    grid-column: span 2; /* Make the email box take up double the space */
  }

/* Additional media query for better responsiveness */
@media (max-width: 768px) {
  .contact-grid {
    grid-template-columns: 1fr; /* Stack items on small screens */
  }
}
@media (max-width: 2608px) {
  .contact-grid {
    grid-template-columns: 1fr; /* Stack items on small screens */
  }

  /* Target the email box specifically */
  .contact-grid {
    grid-column: span 2; /* Make the email box take up double the space */
  }
}


  
  .contact-info p {
    margin-bottom: 15px;
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
 margin-top: 1.5em;
}
  .btn1 {
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
 margin-top: 1.5em;
}
  .btn2 {
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
 margin-top: 1.5em;
}
  .btn3 {
 display: inline-block;
 padding: 0.9rem 1.8rem;
 font-size: 17px;
 font-weight: 200;
 color: white;
 border: .01px solid rgb(255, 255, 255);
 cursor: pointer;
 position: relative;
 background-color: transparent;
 text-decoration: none;
 overflow: hidden;
 z-index: 1;
 font-family: inherit;
 border-radius: 0px;
 margin-top: 1.5em;
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
.btn3::before {
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

.btn3:hover::before {
 transform: translateX(0);
 border-radius: 0px;
 border: none;
}
.btn2::before {
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

.btn2:hover::before {
 transform: translateX(0);
 border-radius: 0px;
 border: none;
}
.btn1::before {
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

.btn1:hover::before {
 transform: translateX(0);
 border-radius: 0px;
 border: none;
}
  
@media (max-width: 768px) {
  .contact-wrapper {
    flex-direction: column;
    text-align: center;
  }

  .contact-form,
  .contact-info {
    width: 100%;
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
  .card {
  /* width: 300px; */
  /* height: 60px; */
  background: black;
  display: flex;
    border: none;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  /* padding: 25px 25px; */
  gap: 20px;
  border-radius: 0px;
  /* margin: 0 auto; */
  /* box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.055); */
}



  
  </style>
  
  