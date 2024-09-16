<template>

   <div>
    <navbar-comp/>
    <about-comp/>
    <skills-comp/>
    <education-comp/>
    <projects-comp/>
    <footer-comp/>

   </div>


 
</template>




<script>
import AboutComp from '@/components/AboutComp.vue';
import EducationComp from '@/components/EducationComp.vue';
import NavbarComp from '@/components/NavbarComp.vue';
import ProjectsComp from '@/components/ProjectsComp.vue';
import SkillsComp from '@/components/SkillsComp.vue';
import FooterComp from '@/components/FooterComp.vue';




export default {
  name: 'HomeView',
  components:{
    NavbarComp,
    AboutComp,
    SkillsComp,
    EducationComp,
    ProjectsComp,
    FooterComp

  }

}
</script>
