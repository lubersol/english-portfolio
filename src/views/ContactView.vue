<script setup>
import { ref, onMounted  } from 'vue'
import { useRouter } from 'vue-router'
import emailjs from '@emailjs/browser'

const formData = ref({
  name: '',
  email: '',
  message: '',
})

const router = useRouter()

const formRef = ref(null)
onMounted(() => {
  // Asigna el formulario al ref después de que el DOM esté listo
  formRef.value = document.getElementById('contactForm')
})

const submitForm = async () => {
  // Datos que se enviarán al servicio de EmailJS
  const emailData = {
    to_email: 'lubersol@gmail.com', 
    from_name: formData.value.name,
    from_email: formData.value.email,
    message: formData.value.message,
  }

  try {
    // Utiliza el ref formRef.value como el tercer parámetro en sendForm
    const response = await emailjs.sendForm('service_3ovhdkp', 'template_86papq3', formRef.value, 'fp1-h6OfHUM6IO3PR')
    console.log('Correo electrónico enviado con éxito', response)
    console.log(emailData)

    // Navegar a la vista 'home' después de enviar el formulario
    router.push({ name: 'home' }) 
  } catch (error) {
    console.error('Error al enviar el correo electrónico', error)
  }
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
        <form ref="form" id="contactForm" @submit.prevent="submitForm" class="contact__form">
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
          <button type="submit" class="btn btn--theme contact__btn">
            Submit
          </button>
        </form>
      </div>
    </div>
  </div>
</template>
