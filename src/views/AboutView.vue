<script setup>
import ButtonItem from '../components/ButtonItem.vue'
import TitleItem from '../components/TitleItem.vue'
import SkillItem from '../components/SkillItem.vue'

</script>

<template>
  <div id="about" class="about sec-pad">
    <div class="main-container">
      <TitleItem title="About Me" subtitle text="Here you will find more information about me, what I do, and my
          current skills mostly in terms of programming and technology">
      </TitleItem>
      <div class="about__content">
        <div class="about__content-main">
          <h3 class="about__content-title">Get to know me!</h3>
          <div class="about__content-details">
            <p class="about__content-details-para">
              I'm a <strong>Fullstack Web Developer</strong> building the
              Front-end of Websites and Web Applications at Affin Solutions company. 
              Check out some of my personal work in the
              <strong>Projects</strong> section.
            </p>
            <p class="about__content-details-para">
              I also like sharing content related to <strong>Web Development</strong>. 
              Feel free to Connect or Follow me on my
              <a rel="noreferrer" href="https://www.linkedin.com/in/luc%C3%ADa-bermejo/" target="_blank">Linkedin</a>
              where I recommend interesting content related to Programming and Web Development.
            </p>
            <p class="about__content-details-para">
              I'm open to <strong>Job</strong> opportunities where I can
              contribute, learn and grow. If you have a good opportunity that
              matches my skills and experience then don't hesitate to
              <strong>contact</strong> me.
            </p>
          </div>
          <ButtonItem text="Contact" href="/contact" />
        </div>
        <SkillItem />
      </div>
    </div>
  </div>
</template>

<style>
.about {
  background: #fafafa;
}
.sec-pad {
  padding:12rem 0;
}
.main-container {
  max-width: 120rem;
  margin: auto;
  width: 92%;
}


@media only screen and (max-width: 56.25em) {
  .sec-pad {
    padding: 8rem 0;
  }
  .heading-sec__mb-med {
    margin-bottom: 8rem;
  }
}
</style>
