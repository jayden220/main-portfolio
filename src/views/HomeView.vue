<template>

   <div>
    <navbar-comp/>
    <home-comp/>

      <section id="about">
        <about-comp/>
      </section>
      <section id="skills">
        <skills-comp/>
      </section>

      <section id="education">
      <education-comp/>
      </section>


      <section id="projects">
        <projects-comp/>
      </section>

      <section id="contact">
        <contact-comp/>
      </section>
    <footer-comp/>

   </div>


 
</template>




<script>
import HomeComp from '@/components/HomeComp.vue';
import AboutComp from '@/components/AboutComp.vue';
import EducationComp from '@/components/EducationComp.vue';
import NavbarComp from '@/components/NavbarComp.vue';
import ProjectsComp from '@/components/ProjectsComp.vue';
import SkillsComp from '@/components/SkillsComp.vue';
import ContactComp from '@/components/ContactComp.vue';
import FooterComp from '@/components/FooterComp.vue';





export default {
  name: 'HomeView',
  components:{
    NavbarComp,
    AboutComp,
    SkillsComp,
    EducationComp,
    ProjectsComp,
    FooterComp,
    HomeComp,
    ContactComp

  }

}
</script>
<style>
section{
  margin-top: 00 ;
}
#contact{
  margin-top: 2em;
}
</style>