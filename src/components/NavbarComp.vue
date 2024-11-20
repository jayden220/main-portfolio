<template>
    <div class="sticky-top">
        <nav class="navbar">
            <p class="brand">J V R</p>
    <div class="container-fluid">
       <nav class="nav-content"> 
        <a href="#">Home</a> |
        <a href="#about">About</a> |
        <a href="#education">Education</a> |
        <a href="#projects">Projects</a> |
        <a href="#contact">Contact</a> 
       </nav>
    </div>
        </nav>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>


.stick-top{
  background-color:black;
}
.navbar{
    color: black;
    background-color: rgba(0, 0, 0, 0.941);
    height: 100px;
    overflow: hidden;
    margin-top: 0;
}

.brand{
  animation: slide 20s infinite alternate;
  font-size: 20px;
  /* position: absolute; */
  /* left: 10px; */
  /* margin-right: 5em; */
}

.nav-conent{
    display: flex;
    justify-content: center;
    margin-bottom: 3em ;
}
.container-fluid{
    display: flex;
    justify-content: center;
}

@keyframes slide {
        100%{
            transform: rotateX(3600deg);
        }
        50%{
          transform: rotateY(360deg);
        }
        40%{
        transform: rotateX(3600deg);
      }
    } 

    .brand{
    display: flex;
    justify-content: center;
    text-decoration: none;
    background: linear-gradient(90deg, #ffbc00, #ff0058);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    }


   a{
    color: aliceblue;
    text-decoration: none;
    font-weight: 400;
    text-transform: uppercase;
    padding: .5em 0;
    font-family: "Bitter";
   } 

 a::before,
 a::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 2px;
  /* color:  linear-gradient(45deg, #ffbc00, #ff0058); */
  background: linear-gradient(45deg, #ffbc00, #ff0058);
  transition: all .5s ease;
  opacity: 0;
  transform: scaleX(0);
  z-index: 1;
}
 a::before {
  top: 1px;
  left: 0;
  transform-origin: left right;
}
 a::after {
  bottom: 2px;
  left: 2px;
  transform-origin: right left;
}
 a:hover::before,
 a:hover::after {
  opacity: 1;
  transform: scaleX(1);
  /* color: #ff0058; */

}
 a:hover {
  color: linear-gradient(90deg, #ffbc00, #ff0058); 
  
  /* filter: blur(30px); */

} 
@media only screen and (max-width: 680px) {
  .brand {
    /* display: flex;
    justify-content: center;
    align-items: center; */
    margin: 0 auto;
  }
}

   @media only screen and (min-width: 684px){
    .brand{
        margin: 0em auto;
    }
    .brand{
        
        animation: 1s bounce infinite both;
    }
    @keyframes bounce {
        100%{
            transform: translateY(2px);
        }
        75%{
            transform: translateY(-2px);
        }
        50%{
            transform: translateY(-1px);
        }
    }
    /* a{
        display: inline-flex;
    } */
   }
</style>

