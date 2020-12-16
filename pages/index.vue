<template>
  <div class="full">
    <div class="grid grid-cols-1 lg:grid-cols-6 gap-4 divide-black divide-x lg:gap-8 m-5 ">
      <div class="p-4 col-span-1 lg:col-span-3 content-center content-between justify-items-center">
        <h1 class="title">der_horst</h1>
        <img src="~/assets/video.png" />
      </div>
      <div class="ter lg:col-span-2"><img src="~/assets/text-m-t.png" /><img src="~/assets/text-m-b.png" /></div>
      <div class="p-4 text-center place-content-between">
        <img src="~/assets/legs.png" />
        <div class="links">
          <a
            href="https://nuxtjs.org/"
            target="_blank"
            rel="noopener noreferrer"
            class="button--grey"
            >
            Der Horst ist eine tolle Wurst
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.full {
  margin: 0 auto;
  min-height: 100vh;
  max-width: 100vw;
  display: flex;
  justify-content: center;
  @apply items-stretch;
  text-align: center;
  @apply h-full;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  letter-spacing: 1px;
  @apply text-black;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  @apply text-black;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
