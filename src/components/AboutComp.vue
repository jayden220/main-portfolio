<template>
    <div class="about-container">
        <div class="about">
            <div class="about-content">
                <h1>Who I Am: A Passionate Developer Ready for New Challenges</h1>
                <p>"Distinguished by a fervent passion for music production and an insatiable curiosity for the ever-evolving realm of computer technology, I am a results-driven individual with a proven track record of excellence. Renowned for my unwavering dedication and tireless work ethic, I thrive in collaborative environments where my enthusiasm for both music and technology can flourish. With a keen eye for detail and a knack for problem-solving, I consistently deliver high-quality outcomes while actively contributing to team success. My journey in the field of technology began with rigorous training and certification from Northlink College, where I honed my skills and solidified my foundation. Currently, I am furthering my expertise at Life Choices coding academy, immersing myself in the intricacies of coding and software development. This dual focus on music production and technology not only fuels my professional aspirations but also fosters a holistic approach to innovation and creativity. I am deeply committed to lifelong learning and continuous improvement, constantly seeking opportunities to expand my knowledge and skill set. With a versatile skill set and a passion for excellence, I am poised to make a significant impact in any endeavor I undertake</p>
            </div>
        </div>
      </div>
</template>
<script>
export default {
    
}
</script>
<style>
    .about-container{
        height: 140vh;
        color: white;
        background-color: rgb(0, 0, 0);
    }
    .about{
        display: flex;
        flex-direction: column;
        text-align: left;
        width: 80%;
        margin: 0 auto;
    }
    .about-content{
  font-size: 24px;
  display: block;
}
@media only screen and (max-width: 767px){
  .about-content{
    font-size: 12px;
  }

}
</style>