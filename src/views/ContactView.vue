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
/* .contact {
  background: linear-gradient(to right,rgba(245,245,245,.8),rgba(245,245,245,.8)),url(/assets/svg/common-bg.svg);
  background-size: cover;
  background-position: center;
}
.sec-pad {
  padding: 12rem 0
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
.heading-sec__main--lt::after {
  content:'';
  background:#7843e9!important;
}
.heading-sec__main::after {
  content:'';
  position:absolute;
  top:calc(100% + 1.5rem);
  height:5px;
  width:3rem;
  background:#7843e9;
  left:50%;
  transform:translateX(-50%);
  border-radius:5px;
}
.heading-sec__sub {
  display:block;
  text-align:center;
  color:#555;
  font-size:2rem;
  font-weight:500;
  max-width:80rem;
  margin:auto;
  line-height:1.6;
}
.heading-sec__sub--lt {
  color:#333;
}
.heading-sec__mb-med {
  margin-bottom:9rem;
} */
/* .contact__form-container {
  box-shadow: rgba(100,100,111,.2) 0 7px 29px 0;
  background: #fff;
  padding: 4rem;
  margin-top: 6rem;
  max-width: 80rem;
  text-align: right;
  width: 95%;
  border-radius: 5px;
  margin: 5rem auto 0 auto;
}
.btn {
  background:#7843e9;
  color:#fff;
  text-transform:uppercase;
  letter-spacing:1px;
  display:inline-block;
  font-weight:700;
  border-radius:5px;
  box-shadow:0 5px 15px 0 rgba(0,0,0,.15);
  transition:transform .3s;
} */
/* .btn:hover {
    transform:translateY(-3px);
}
.btn--theme {
    background:#7843e9;
    color:#fff;
}
.contact__form-field {
  margin-bottom: 4rem;
}
.contact__form-label {
  color: #666;
  font-size: 1.4rem;
  letter-spacing: 1px;
  font-weight: 700;
  margin-bottom: 1rem;
  display: block;
  text-align: left;
} */

/* .contact__form-input {
  color: #333;
  padding: 2rem;
  width: 100%;
  border: 1px solid #ebebeb;
  font-size: 1.6rem;
  letter-spacing: 0;
  background: #f0f0f0;
  border-radius: 5px;
  font-weight: 600;
}

.contact__form-input::-moz-placeholder {
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
} */

/* .contact__form-input:-ms-input-placeholder {
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
}

.contact__form-input::placeholder {
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
}

.contact__form-input::-webkit-input-placeholder {
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
}

.contact__form-input:-ms-input-placeholder {
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
}

.contact__form-input::-ms-input-placeholder {
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
}

.contact__form-input:-moz-placeholder {
  opacity: 1;
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
}

.contact__form-input::-moz-placeholder {
  opacity: 1;
  color: #999;
  font-weight: 600;
  font-size: 1.6rem;
}

.contact__btn {
  width: 30%;
  padding: 2rem 4rem;
  font-size: 1.6rem;
} */

/* @media only screen and (max-width: 56.25em) {
  .sec-pad {
    padding: 8rem 0;
  }
  .heading-sec__mb-med {
    margin-bottom: 8rem;
  }
}
@media only screen and (max-width:37.5em) {
  .heading-sec__main::after {
    top:calc(100% + 1.2rem);
  }
  .heading-sec__sub {
    font-size:1.8rem;
  }
  .contact__form-container {
    padding: 3rem;
  }
  .contact__form-field {
    margin-bottom: 3rem;
  }
  .contact__btn {
      width:100%;
  }
} */

</style>
