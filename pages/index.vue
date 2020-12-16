<template>
  <div class="full">
    <div class="grid grid-cols-1 lg:grid-cols-12 gap-4 divide-black divide-x-2 lg:gap-8 m-5">
      <div class="p-4 col-span-1 lg:col-span-5 px-8 flex flex-col justify-between">
        <h1 class="title">der_horst</h1>
        <img class="flex-initial lg:px-24" src="~/assets/video.png" />
      </div>
      <div class="text-center lg:col-span-4 px-8 flex flex-col justify-between"><img src="~/assets/text-m-t.png" /><img class="object-bottom" src="~/assets/text-m-b.png" /></div>
      <div class="col-span-1 lg:col-span-3 p-4 text-center flex flex-col justify-between">
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

.divide-x-3 {
  --tw-divide-x-reverse: 0;
  border-right-width: calc(2px * var(--tw-divide-x-reverse));
  border-left-width: calc(2px * calc(1 - var(--tw-divide-x-reverse)));
}

.marign-zero{
  margin: 0 auto;
}
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
