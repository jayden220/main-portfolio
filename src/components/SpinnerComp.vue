
<template>
    <div class="spinner-container">

        <div class="loader">
      
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
/* From Uiverse.io by alexruix */ 
.loader {
  position: relative;
  margin: auto;
  box-sizing: border-box;
  background-clip: padding-box;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  border: 4px solid rgba(255, 255, 255, 0.1);
  -webkit-mask:linear-gradient(90deg, #ffbc00, #ff0058);
  background: linear-gradient(90deg, #ffbc00, #ff0058);

  transform-origin: 50% 60%;
  transform: perspective(200px) rotateX(66deg);
}

.loader:before, .loader:after {
  content: "";
  position: absolute;
  margin: -4px;
  box-sizing: inherit;
  width: inherit;
  height: inherit;
  border-radius: inherit;
  opacity: 0.05;
  border: inherit;
  border-color: transparent;
  animation: spinner-spin 1.2s cubic-bezier(0.6, 0.2, 0, 0.8) infinite, spinner-fade 1.2s linear infinite;
}

.loader:before {
  border-top-color: #ffbc00;
}

.loader:after {
  border-top-color: #ff0058;
  animation-delay: 0.3s;
}

@keyframes spinner-spin {
  100% {
    transform: rotate(360deg);
  }
}

@keyframes spinner-fade {
  20% {
    opacity: 0.1;
  }

  40% {
    opacity: 1;
  }

  60% {
    opacity: 0.1;
  }
}
 
</style>