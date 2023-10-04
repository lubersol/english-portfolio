<template>
    <div class="main-container">
      <div class="main-footer__upper">
        <div class="main-footer__row main-footer__row-1">
          <h2 class="heading heading-sm main-footer__heading-sm">
            <span>Social</span>
          </h2>
          <div class="main-footer__social-cont">
            <a target="_blank" rel="noreferrer" href="https://www.linkedin.com/in/luc%C3%ADa-bermejo/">
                <i class="fab fa-linkedin" style="font-size: large;" title="LinkedIn"></i>
            </a>
            <a target="_blank" rel="noreferrer" href="https://github.com/lubersol">
              <i class="fab fa-github" style="font-size: large;" title="Github"></i>
            </a>
            <a target="_blank" rel="noreferrer" href="https://drive.google.com/file/d/1kBPe6RL3Vn-fe6zkrT69YsUX1lyXZwZV/view?usp=sharing">
              <i class="fa-solid fa-file" style="font-size: large;" title="Mi CV"></i>
            </a>
          </div>
        </div>
        <div class="main-footer__row main-footer__row-2">
          <h2 class="heading heading-sm text-lt">Lucía Bermejo</h2>
          <p class="main-footer__short-desc">
            A Full Stack focused Web Developer building the Frontend of Websites
            and Web Applications that leads to the success of the overall
            product
          </p>
        </div>
      </div>
    </div>
</template>

<style scoped>
.main-container {
  max-width:120rem;
  margin:auto;width:92%;
}
.main-footer__upper {
  display:flex;
  justify-content:space-between;
  padding:8rem 0;
}
.main-footer__row-1 {
  order:2;
}
.main-footer__row-2 {
  width:40%;
  order:1;
  max-width:50rem;
}
.main-footer__short-desc{
  margin-top:2rem;
  color:#eee;
  font-size:1.5rem;
  line-height:1.7;
}
.main-footer__social-cont{
  display: flex;
  justify-content: space-around;
  margin-top:2rem;
}

@media only screen and (max-width:56.25em){
    .main-footer__upper{
        padding:6rem 0;
    }
    .main-footer__row-1{
        margin-bottom:5rem;
    }
    .main-footer__row-2{
        width:100%;
    }
}
@media only screen and (max-width:37.5em){
    .main-footer__upper{
        display:block
    }
}

</style>