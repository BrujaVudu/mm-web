<template lang="pug">
main
  .intro
    NuxtLink(to="https://docs.google.com/forms/d/e/1FAIpQLSdWV74Zjq8UZAiuMlEK8x2T67k67Vru-Kayu09FnQL7Yy28vg/viewform")
      img(src='/texto.png')
    .contacto
      NuxtLink(to="https://youtube.com/@magicmarkerspro" title="Ver nuestros videos" target="_blank" class="tooltip")
        span(class="tooltiptext")  Ver nuestros videos
        img(src="/yt.svg")
      NuxtLink(to="https://instagram.com/magicmarkerspro" title="Instagram Magic Markers" target="_blank" class="tooltip")
        span(class="tooltiptext") Instagram
        img(src="/ig.svg")
      NuxtLink(to="mailto:contacto@magicmarkers.tv" title="Escríbenos un correo" target="_blank" class="tooltip")
        span(class="tooltiptext") Escríbenos
        img(src="/mail.svg")
        
  // menu
      NuxtLink(to="https://youtube.com/@magicmarkerspro" title="Ver nuestros videos" target="_blank")
        img(src="/Videos.png")  
      img(src="/Nosotros.png" onclick="alert('ups, esto está en construcción')")
      img(src="/Clientes.png" onclick="alert('ups, esto está en construcción')")
</template>
<style lang="sass">
html, #__nuxt, #__nuxt > div
  height: 100%
body
  background: url('/bg.webp') no-repeat center center/cover
  background-attachment: fixed
  color: black
  height: 100%
  margin: 0
  padding: 0
.intro
  display: flex
  align-items: center
  justify-content: center
  flex-direction: column
  gap: 40px
  height: calc(100vh + 40px)
menu
  display: flex
  flex-direction: column
  margin: 0
  padding: 0 
  img
    width: fit-content
    max-width: 90vw
    mix-blend-mode: multiply
    margin-top: calc(-1 * min(40px, 5vw))
    
img
  max-width: 94vw
.contacto
  display: flex
  gap: 20px
.tooltip
  position: relative
  display: inline-block

  .tooltiptext
    font-family: sans-serif
    visibility: hidden
    width: max-content
    background-color: black
    color: #fff
    text-align: center
    padding: 4px 6px
    border-radius: 6px
    position: absolute
    top: -40px
    z-index: 1

  &:hover .tooltiptext
    visibility: visible
</style>