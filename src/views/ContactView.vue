<template>
  <div id="contact" class="contact sec-pad dynamicBg">
    <div class="main-container">
      <h2 class="heading heading-sec heading-sec__mb-med">
        <span class="heading-sec__main heading-sec__main--lt">Contact</span>
        <span class="heading-sec__sub heading-sec__sub--lt">
          Feel free to Contact me by submitting the form below and I will get
          back to you as soon as possible
        </span>
      </h2>
      <div class="contact__form-container">
        <form action="#" class="contact__form" method="post"><input type="hidden" name="form-name" value="form 1">
          <div class="contact__form-field">
            <label class="contact__form-label" for="name">Name</label>
            <input required placeholder="Enter Your Name" type="text" class="contact__form-input" name="name" id="name">
          </div>
          <div class="contact__form-field">
            <label class="contact__form-label" for="email">Email</label>
            <input required placeholder="Enter Your Email" type="email" class="contact__form-input" name="email" id="email">
          </div>
          <div class="contact__form-field">
            <label class="contact__form-label" for="message">Message</label>
            <textarea required cols="30" rows="10" class="contact__form-input" placeholder="Enter Your Message" name="message" id="message"></textarea>
          </div>
          <button type="submit" class="btn btn--theme contact__btn">
            Submit
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<style>
.contact {
  background: linear-gradient(to right,rgba(245,245,245,.8),rgba(245,245,245,.8)),url(/daac885…/c157c/assets/svg/common-bg.svg);
  background-size: cover;
  background-position: center;
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
.heading-sec__main--lt {
  color: #111;
  font-weight: 800;
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
