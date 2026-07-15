<script setup>
const sendMail = (event) => {
  event.preventDefault()

  const name = event.target.name.value
  const email = event.target.email.value
  const message = event.target.message.value

  const subject = encodeURIComponent("Steam Website Inquiry")

  const body = encodeURIComponent(
`Name: ${name}

Email: ${email}

Message:
${message}`)
  
  window.location.href =
    `mailto:kcg@up-pad.com?subject=${subject}&body=${body}`
}
</script>

<template>

<section class="contact" id="contact">

    <h2>お問い合わせ</h2>

    <p class="contact-text">
        Have questions or feedback?
        We'd love to hear from you.
    </p>

    <form @submit="sendMail">

        <input
            type="text"
            name="name"
            placeholder="Your Name"
            required
        >

        <input
            type="email"
            name="email"
            placeholder="Your Email"
            required
        >

        <textarea
            name="message"
            rows="6"
            placeholder="Your Message"
            required
        ></textarea>

        <button type="submit">
            Send Message
        </button>

    </form>

</section>

</template>

<style scoped>

</style>