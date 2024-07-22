<template lang="pug">
.centrar
  NuxtLink(to="https://docs.google.com/forms/d/e/1FAIpQLSdWV74Zjq8UZAiuMlEK8x2T67k67Vru-Kayu09FnQL7Yy28vg/viewform")
    img(src='/texto.png')
  .contacto
    NuxtLink(to="https://youtube.com/@magicmarkerspro" title="Ver nuestros videos")
      img(src="/yt.svg")
    NuxtLink(to="https://instagram.com/magicmarkerspro" title="Instagram Magic Markers")
      img(src="/ig.svg")
    NuxtLink(to="mailto:contacto@magicmarkersp.tv" title="Escríbenos un correo")
      img(src="/mail.svg")
</template>
<style lang="sass">
html, #__nuxt, #__nuxt > div
  height: 100%
body
  background: url('/bg.webp') no-repeat center center/cover
  color: black
  height: 100%
  margin: 0
  padding: 0
.centrar
  display: flex
  align-items: center
  justify-content: center
  flex-direction: column
  gap: 40px
  height: 100%
img
  max-width: 94vw
.contacto
  display: flex
  gap: 20px
</style>