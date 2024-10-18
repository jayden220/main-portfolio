<template>
  <div class="project-container">
    <h3 class="heading">My work</h3>
    <div class="project-list">
        <div class="card">
          <div class="first-content">
            <span>First</span>
            <h3></h3>
          </div>
          <div class="second-content">
        <span>Second</span>
          </div>
        </div>

        <div class="card">
          <div class="first-content">
            <span>First</span>
          </div>
          <div class="second-content">
        <span>Second</span>
          </div>
        </div>
      


 
  </div>
  </div>
</template>

<script>
export default {
  // ...
};
</script>

<style scoped>
.heading {
  /* margin: 3em 3em; */
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
  background: rgb(103, 225, 255);
  transition: all 0.4s;
  border-radius: 10px;
  box-shadow: 0px 0px 10px 5px  rgba(0, 0, 0, 0.705);
  font-size: 30px;
  font-weight: 900;
}

.card:hover {
  border-radius: 15px;
  cursor: pointer;
  transform: scale(1.2);
  box-shadow: 0px 0px 10px 5px  rgba(0, 0, 0, 0.705);
  background: rgb(103, 151, 255);
}

.first-content {
  height: 100%;
  width: 100%;
  transition: all 0.4s;
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 1;
  border-radius: 15px;
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
  justify-content: center;
  align-items: center;
  border-radius: 15px;
  transition: all 0.4s;
  font-size: 0px;
  transform: rotate(90deg) scale(-1);
}

.card:hover .second-content {
  opacity: 1;
  height: 100%;
  font-size: 1.8rem;
  transform: rotate(0deg);
}


.p-image {
  margin: 2em 0;
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