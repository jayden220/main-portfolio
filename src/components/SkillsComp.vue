<template >
    <div class="main-container">
        <h2> Technical skills</h2>
        <div class="tech-skills">
            <div class="card">
                    <span></span>
                <div class="content">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" alt="" >
                </div>
            </div>
           
            <div class="card">
                    <span></span>
                <div class="content">
                        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="" >
                </div>
            </div>
            <div class="card">
                    <span></span>
                <div class="content">
                        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-original-wordmark.svg" alt="" >
                </div>
            </div>
            <div class="card">
                    <span></span>
                <div class="content">
                        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="" >
                </div>
            </div>
            <div class="card">
                    <span></span>
                <div class="content">
                        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original-wordmark.svg" alt="" >
                </div>
            </div>
            <div class="card">
                    <span></span>
                <div class="content">
                        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original-wordmark.svg" alt="" >
                </div>
            </div>
            <div class="card">
                    <span></span>
                <div class="content">
                        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original-wordmark.svg" alt="" >
                </div>
            </div>
            <div class="card">
                    <span></span>
                <div class="content">
                        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/azuresqldatabase/azuresqldatabase-original.svg" alt="" >
                </div>
            </div>
        </div>
        <!-- end of Tech skills container -->
         <div class="softskills">

         </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    .main-container{
        height: fit-content;
        background-color: rgb(0, 0, 0);
    }
    .tech-skills{
        display:grid;
        grid-template-columns: repeat(auto-fit, minmax(20cqi,1fr)) ;
        place-items: center;
        gap: 1.5cqi;
    }
    img{
        height: 6em;
    }

.card {
  position: relative;
  width: 190px;
  /* height: 254px; */
  color: #fff;
  transition: 0.5s;
  border-radius: 20px;
  cursor: pointer;
  margin: 1em 0 ;
}

.card:hover {
  transform: translateY(-20px);
}

.card::before {
  content: '';
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  background: linear-gradient(45deg, #ffbc00, #ff0058);
  border-radius: 1.2em;
}

.card::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(45deg, #ffbc00, #ff0058);
  filter: blur(30px);
}

.card span {
  position: absolute;
  top: 6px;
  left: 6px;
  right: 6px;
  bottom: 6px;
  /* background-color: rgba(0, 0, 0, 0.789); */
  z-index: 2;
  border-radius: 1em;
}

.card span::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 50%;
  height: 100%;
  /* background-color: rgba(229, 15, 15, 0.1); */
}

.card .content {
  position: relative;
  padding: 10px;
  z-index: 10;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 800;
  font-size: 1.5em;
}
</style>