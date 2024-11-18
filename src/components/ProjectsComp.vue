<template>
  <div class="project-container">
    <h3 class="heading">My work</h3>
    <div class="project-list">
        <div class="card" v-for="project in projects" :key="project.name">
          <div class="first-content">
            <span></span>
            <h3>{{ project.name }}</h3> <!-- Display project name -->
          </div>
          <div class="second-content">
            <span></span>
            <img :src="project.image" alt="Project image" /> <!-- Display project image -->
            <br><br>
            <p>{{ project.description }}</p> <!-- Display project description -->
            <div class="button-group">
            <a :href="project.github" target="_blank"><button class="btn">
              <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="23" height="21" viewBox="0 0 50 50">
    <path d="M17.791,46.836C18.502,46.53,19,45.823,19,45v-5.4c0-0.197,0.016-0.402,0.041-0.61C19.027,38.994,19.014,38.997,19,39 c0,0-3,0-3.6,0c-1.5,0-2.8-0.6-3.4-1.8c-0.7-1.3-1-3.5-2.8-4.7C8.9,32.3,9.1,32,9.7,32c0.6,0.1,1.9,0.9,2.7,2c0.9,1.1,1.8,2,3.4,2 c2.487,0,3.82-0.125,4.622-0.555C21.356,34.056,22.649,33,24,33v-0.025c-5.668-0.182-9.289-2.066-10.975-4.975 c-3.665,0.042-6.856,0.405-8.677,0.707c-0.058-0.327-0.108-0.656-0.151-0.987c1.797-0.296,4.843-0.647,8.345-0.714 c-0.112-0.276-0.209-0.559-0.291-0.849c-3.511-0.178-6.541-0.039-8.187,0.097c-0.02-0.332-0.047-0.663-0.051-0.999 c1.649-0.135,4.597-0.27,8.018-0.111c-0.079-0.5-0.13-1.011-0.13-1.543c0-1.7,0.6-3.5,1.7-5c-0.5-1.7-1.2-5.3,0.2-6.6 c2.7,0,4.6,1.3,5.5,2.1C21,13.4,22.9,13,25,13s4,0.4,5.6,1.1c0.9-0.8,2.8-2.1,5.5-2.1c1.5,1.4,0.7,5,0.2,6.6c1.1,1.5,1.7,3.2,1.6,5 c0,0.484-0.045,0.951-0.11,1.409c3.499-0.172,6.527-0.034,8.204,0.102c-0.002,0.337-0.033,0.666-0.051,0.999 c-1.671-0.138-4.775-0.28-8.359-0.089c-0.089,0.336-0.197,0.663-0.325,0.98c3.546,0.046,6.665,0.389,8.548,0.689 c-0.043,0.332-0.093,0.661-0.151,0.987c-1.912-0.306-5.171-0.664-8.879-0.682C35.112,30.873,31.557,32.75,26,32.969V33 c2.6,0,5,3.9,5,6.6V45c0,0.823,0.498,1.53,1.209,1.836C41.37,43.804,48,35.164,48,25C48,12.318,37.683,2,25,2S2,12.318,2,25 C2,35.164,8.63,43.804,17.791,46.836z"></path>
</svg>

          </button></a> <!-- Link to GitHub -->
              <a :href="project.vercel" target="_blank"><button class="btn">Live</button></a> <!-- Link to Live Demo -->
            </div>
          </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      "projects":[
        {
            "name":"Calculator",    
            "github":"https://github.com/jayden220/calculator-project.git",
            "vercel":"https://calculator-project-wine.vercel.app/",
            "description":"I used Javascript, CSS and HTML to create a functional calculator",
            "image":"https://jayden220.github.io/hostedImages/images/Screenshot%202024-07-03%20095121.png"
        },
        {
            "name":"Hulu Clone",
            "github":"https://github.com/jayden220/hulu-clone-project.git",
            "vercel":"https://hulu-clone-project-omega.vercel.app/",
            "description":"This is an HTML project where I created a clone of the HULU streaming website",
            "image":"https://jayden220.github.io/hostedImages/images/Screenshot%202024-07-03%20095057.png"
        },
        {
            "name":"Temp Converter",
            "github":"https://github.com/jayden220/TempCon.git",
            "vercel":"https://temp-con.vercel.app/",
            "description":"This is a JavaScript project where a user inputs the temperature in celcius and it converts to farenheit",
            "image":"https://jayden220.github.io/hostedImages/images/Screenshot%202024-07-03%20095140.png"
        },
        {
            "name":"E-Commerce",
            "github":"https://github.com/jayden220/JavaScript-Project.git",
            "vercel":"https://java-script-project-rho.vercel.app/",
            "description":"In this project I created a basic design for my portfolio using CSS and HTML",
            "image":"https://jayden220.github.io/hostedImages/images/Screenshot%202024-07-03%20094652.png"
        },
        {
            "name":"Age To Days",
            "github":"https://github.com/jayden220/Years2days.git",
            "vercel":"https://years2days.vercel.app/",
            "description":"This is a JavaScript project where a user inputs any age in years and it converts to days",
            "image":"https://jayden220.github.io/hostedImages/images/Screenshot%202024-07-03%20094856.png"
        },
        {
            "name":"Keyboard",
            "github":"https://github.com/jayden220/keyboard.git",
            "vercel":"https://keyboard-project-nine.vercel.app/",
            "description":"In this project a created a wood design keyboard using HTML and CSS",
            "image":"https://jayden220.github.io/hostedImages/images/Screenshot%202024-07-03%20095025.png"
        },
        {
            "name":"RGB To Hexadecimal",
            "github":"https://github.com/jayden220/RGB2HEX.git",
            "vercel":"https://rgb-2-hex.vercel.app/",
            "description":"This is a converter that changes RGB color codes into a Hexadecimal value",
            "image":"https://jayden220.github.io/hostedImages/images/Screenshot%202024-07-03%20095210.png"
        }
    ]
    }
  }
};
</script>

<style scoped>
.heading {
  margin-top: 4em;
  font-size: 3em;
  color: white;
}

.project-container {
  background-color: black;
  min-height: 100vh; /* Use min-height instead of fixed height */
  margin-top: 0em;
  overflow-y: hidden;
  display: flex;
  flex-direction: column; /* Stack heading and project list */
  align-items: center; /* Center content horizontally */
}

.project-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: flex-start; /* Align items at the start */
  gap: 5em;
  padding: 2em; /* Add padding for better spacing */
}

/* .card {
  width: 390px;
  height: 354px;
  transition: all 0.3s ease;
  margin-bottom: 1em;
} */
/* From Uiverse.io by suleymanlaarabidev */ 
.card {
  width: 190px;
  height: 254px;
  background: rgb(7, 7, 7);
  transition: all 0.4s;
  border-radius: 0px;
  box-shadow: 0px 0px 10px 5px  rgba(0, 0, 0, 0.705);
  font-size: 30px;
  font-weight: 900;
}
/* img{
  width: 100%;
  height: 50%;
} */
img {
  width: 100%; /* Make the image responsive */
  max-width: 200px; /* Maintain max size */
  /* margin-top: 3em; */
  height: auto; /* Maintain aspect ratio */
}

.card:hover {
  /* border-radius: 15px; */
  cursor: pointer;
  transform: scale(1.2);
  box-shadow: 0px 0px 10px 5px  rgba(0, 0, 0, 0.705);
  background: rgb(28, 30, 34);
}

.first-content {
  height: 100%;
  width: 100%;
  transition: all 0.4s;
  display: flex;
  color: white;
  background: linear-gradient(90deg, #ffbc00, #ff0058);
  justify-content: center;
  align-items: center;
  opacity: 1;
  /* border-radius: 15px; */
}

.card:hover .first-content {
  height: 0px;
  opacity: 0;
}

.second-content {
  height: 0%;
  width: 100%;
  opacity: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* border-radius: 15px; */
  transition: all 0.8s;
  font-size: 1px;
  color: #ffffff;
  transform: rotate(90deg) scale(-1);
}

.card:hover .second-content {
  opacity: 1;
  height: 100%;
  font-size: .8rem;
  transform: rotate(0deg);
}
.button-group{
  display: flex;
  justify-content:space-between ;
  gap: 2em;

}
/* From Uiverse.io by joe-watson-sbf */ 
.btn {
 /* display: inline-block; */
 padding: 0.9rem 1.8rem;
 font-size: 16px;
 font-weight: 700;
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
 gap: 2em
 ;
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
}



.project-btn {
  background-color: transparent;
  /* margin-right: 1em; */
}

.talk-btn {
  border: none;
}



.p-image {
  margin: 2em 1em;
  width: 200px;
  height: 200px;
}

@media (min-width: 1024px) {
  .card {
    width: 450px; /* Increase card width for larger screens */
    height: 400px; /* Increase card height for larger screens */
  }

  .heading {
    font-size: 4em; /* Increase heading size */
  }

  .project-list {
    gap: 4em; /* Adjust gap between cards */
  }
}

@media (max-width: 480px) {
  .card {
    width: 90%; /* Make cards responsive on small screens */
    margin: 0 2em;
  }
}

@keyframes floating {
  0% {
    transform: translateY(0px);
  }
  50% {
 transform: translateY(-10px);
  }
  100% {
    transform: translateY(0px);
  }
}
</style>