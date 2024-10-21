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
            <div>
            <a :href="project.github" target="_blank"><button class="btn">
            <svg viewBox="0 0 128 128">
            <g fill="#181616"><path fill-rule="evenodd" clip-rule="evenodd" d="M64 5.103c-33.347 0-60.388 27.035-60.388 60.388 0 26.682 17.303 49.317 41.297 57.303 3.017.56 4.125-1.31 4.125-2.905 0-1.44-.056-6.197-.082-11.243-16.8 3.653-20.345-7.125-20.345-7.125-2.747-6.98-6.705-8.836-6.705-8.836-5.48-3.748.413-3.67.413-3.67 6.063.425 9.257 6.223 9.257 6.223 5.386 9.23 14.127 6.562 17.573 5.02.542-3.903 2.107-6.568 3.834-8.076-13.413-1.525-27.514-6.704-27.514-29.843 0-6.593 2.36-11.98 6.223-16.21-.628-1.52-2.695-7.662.584-15.98 0 0 5.07-1.623 16.61 6.19C53.7 35 58.867 34.327 64 34.304c5.13.023 10.3.694 15.127 2.033 11.526-7.813 16.59-6.19 16.59-6.19 3.287 8.317 1.22 14.46.593 15.98 3.872 4.23 6.215 9.617 6.215 16.21 0 23.194-14.127 28.3-27.574 29.796 2.167 1.874 4.097 5.55 4.097 11.183 0 8.08-.07 14.583-.07 16.572 0 1.607 1.088 3.49 4.148 2.897 23.98-7.994 41.263-30.622 41.263-57.294C124.388 32.14 97.35 5.104 64 5.104z"></path><path d="M26.484 91.806c-.133.3-.605.39-1.035.185-.44-.196-.685-.605-.543-.906.13-.31.603-.395 1.04-.188.44.197.69.61.537.91zm2.446 2.729c-.287.267-.85.143-1.232-.28-.396-.42-.47-.983-.177-1.254.298-.266.844-.14 1.24.28.394.426.472.984.17 1.255zM31.312 98.012c-.37.258-.976.017-1.35-.52-.37-.538-.37-1.183.01-1.44.373-.258.97-.025 1.35.507.368.545.368 1.19-.01 1.452zm3.261 3.361c-.33.365-1.036.267-1.552-.23-.527-.487-.674-1.18-.343-1.544.336-.366 1.045-.264 1.564.23.527.486.686 1.18.333 1.543zm4.5 1.951c-.147.473-.825.688-1.51.486-.683-.207-1.13-.76-.99-1.238.14-.477.823-.7 1.512-.485.683.206 1.13.756.988 1.237zm4.943.361c.017.498-.563.91-1.28.92-.723.017-1.308-.387-1.315-.877 0-.503.568-.91 1.29-.924.717-.013 1.306.387 1.306.88zm4.598-.782c.086.485-.413.984-1.126 1.117-.7.13-1.35-.172-1.44-.653-.086-.498.422-.997 1.122-1.126.714-.123 1.354.17 1.444.663zm0 0"></path></g>
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
img{
  width: 100%;
  height: 50%;
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
/* From Uiverse.io by joe-watson-sbf */ 
.btn {
  font-size: 17px;
  background: transparent;
  border: none;
  padding: 1em 1.5em;
  color: #ffffff;
  text-transform: uppercase;
  position: relative;
  transition: 0.5s ease;
  cursor: pointer;
}

.btn::before {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  height: 2px;
  width: 0;
  background: linear-gradient(90deg, #ffbc00, #ff0058);
  /* background-color: #ffc506; */
  
  transition: 0.5s ease;
}

.btn:hover {
  color: #1e1e2b;
  transition-delay: 0.5s;
}

.btn:hover::before {
  width: 100%;
}

.btn::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  height: 0;
  width: 100%;
  background: linear-gradient(90deg, #ffbc00, #ff0058);
  /* background-color: #ffc506; */
  transition: 0.4s ease;
  z-index: -1;
}

.btn:hover::after {
  height: 100%;
  transition-delay: 0.4s;
  color: aliceblue;
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