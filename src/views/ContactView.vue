<script setup>
import { ref } from 'vue'
import emailjs from '@emailjs/browser'

const formData = ref({
  name: '',
  email: '',
  message: '',
})
const submitForm = async () => {
  // Datos que envío al servicio de EmailJS
  const emailData = {
    to_email: 'lubersol@gmail.com', 
    from_name: formData.value.name,
    from_email: formData.value.email,
    message: formData.value.message,
  }

  try {
    // Envía el correo electrónico
    const response = await emailjs.sendForm('service_3ovhdkp', 'template_86papq3', emailData, 'fp1-h6OfHUM6IO3PR')
    console.log('Correo electrónico enviado con éxito', response)
  } catch (error) {
    console.error('Error al enviar el correo electrónico', error)
  }
}

const toHome = () => {
  window.$nuxt.$router.push('/')
}
</script>

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
        <form ref="formData" id="contactForm" @submit.prevent="submitForm" class="contact__form">
          <input type="hidden" name="form-name" value="form 1">
          <div class="contact__form-field">
            <label class="contact__form-label" for="name">Name</label>
            <input required placeholder="Enter Your Name" type="text" class="contact__form-input" name="name" id="name" v-model="formData.name">
          </div>
          <div class="contact__form-field">
            <label class="contact__form-label" for="email">Email</label>
            <input required placeholder="Enter Your Email" type="email" class="contact__form-input" name="email" id="email" v-model="formData.email">
          </div>
          <div class="contact__form-field">
            <label class="contact__form-label" for="message">Message</label>
            <textarea required cols="30" rows="10" class="contact__form-input" placeholder="Enter Your Message" name="message" id="message" v-model="formData.message"></textarea>
          </div>
          <button type="submit" class="btn btn--theme contact__btn" @click="toHome">
            Submit
          </button>
        </form>
      </div>
    </div>
  </div>
</template>
