<script setup>
import ButtonItem from '../components/ButtonItem.vue'
import TitleItem from '../components/TitleItem.vue'
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
        <div class="about__content-skills">
          <h3 class="about__content-title">My Skills</h3>
          <div class="skills">
            <div class="skills__skill">HTML</div>
            <div class="skills__skill">CSS</div>
            <div class="skills__skill">JavaScript</div>
            <div class="skills__skill">React</div>
            <div class="skills__skill">VUE</div>
            <div class="skills__skill">Pinia</div>
            <div class="skills__skill">Jest</div>
            <div class="skills__skill">GIT</div>
            <div class="skills__skill">Github</div>
            <div class="skills__skill">NodeJS</div>
            <div class="skills__skill">Express</div>
            <div class="skills__skill">PHP</div>
            <div class="skills__skill">Laravel</div>
            <div class="skills__skill">SQL</div>
            <div class="skills__skill">MongoDB</div>
            <div class="skills__skill">Terminal</div>
            <div class="skills__skill">Responsive Design</div>
            <div class="skills__skill">SEO</div>
            <div class="skills__skill">SASS</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.about {
  background: #fafafa;
}
.main-container {
  max-width: 120rem;
  margin: auto;
  width: 92%;
}
.heading-sec__main {
  display: block;
  font-size: 4rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  letter-spacing: 3px;
  text-align: center;
  margin-bottom: 3.5rem;
  position: relative;
  color: #111;
}
.heading-sec__sub {
  display: block;
  text-align: center;
  color: #555;
  font-size: 2rem;
  font-weight: 500;
  max-width: 80rem;
  margin: auto;
  line-height: 1.6;
}
.about__content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 10rem;
}
@media only screen and (max-width: 56.25em) {
  .sec-pad {
    padding: 8rem 0;
  }
  .heading-sec__mb-med {
    margin-bottom: 8rem;
  }
  .about__content {
    grid-template-columns: 1fr;
    grid-gap: 8rem;
  }
}
</style>
