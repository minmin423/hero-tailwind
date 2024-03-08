<script setup>
import { Icon } from '@iconify/vue';
</script>

<template>
  <div class="w-full p-2 lg:px-10 py-5 min-h-screen bg-gray-100 font-bold font-roboto">
    
    <!-- NAVIGATION BAR -->
    <nav class="flex h-full justify-between bg-white rounded-full p-5 font-bold">
      <!-- LOGO -->
      <div class="flex gap-1 items-center">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6f/Logo_of_Twitter.svg/512px-Logo_of_Twitter.svg.png" class="w-10 h-10" alt="">
        <div class="text-xl">tweety</div>
      </div>

      <!-- Navigation Links -->
      <ul class=" hidden lg:flex gap-8 items-center">
        <li v-for="(item, index) in ['Features', 'Solutions', 'Resources', 'Pricing']"
        :key="index">{{ item }}</li>
      </ul>

      <!-- Buttons -->
      <div class="hidden lg:flex gap-4">
        <button @click.prevent="" class="py-2 p-4 border rounded-full">Log In</button>
        <button @click.prevent="" class="py-2 p-4 border rounded-full font-semibold bg-blue-500 text-white">Get Started</button>
      </div>
      
      <div class="lg:hidden h-full flex items-center">
        <button @click.prevent=""><Icon icon="mingcute:menu-fill" class="h-10 w-10" /></button>
      </div>
    </nav>

    <!-- HERO -->
    <main class="w-full flex h-full flex-col-reverse lg:flex-row lg:gap-[20vw] justify-between pt-10 lg:pt-20 pb-20">
      <!-- CONTENT -->
      <div class="w-full lg:w-1/2 flex flex-col justify-between gap-8 pt-10 lg:pt-0 text-center lg:text-start">
        <div class="flex flex-col just gap-6">
          <h2 class="uppercase text-blue-500">Best Caption Here</h2>
          <h1 class="text-5xl lg:text-6xl">Build online business from home.</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus error beatae fuga quos assumenda deleniti veniam vitae commodi unde? Nostrum voluptatem minus facere repellat facilis eligendi molestiae iusto eum possimus.</p>

          <div class="flex gap-10">
            <div class="flex w-full gap-10 lg:gap-2 lg:justify-start">
              <button @click.prevent="" class="w-full py-2 px-4 border rounded-full font-semibold bg-blue-500 text-white text-sm whitespace-nowrap">Get Started</button>
              <button @click.prevent="" class="w-full py-2 px-4 rounded-full bg-white text-sm whitespace-nowrap">Watch Video</button>
            </div>

            <div class="hidden lg:block w-full"></div>
          </div>
        </div>

        <!-- Review Cards -->
        <div class="flex w-full justify-center gap-10">
          <div class="flex flex-col w-1/2 items-start gap-2 bg-white rounded-xl p-4 lg:p-8">
            <div class="flex">
              <Icon v-for="index in 5" :key="index" icon="ic:round-star" class="w-6 h-6 text-green-600" />
            </div>

            <div>4.2/5 <span class="text-gray-400 font-normal">(45k Reviews)</span></div>

            <div>
                <img class="w-2/3" src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/78/Trustpilot_Logo_%282022%29.svg/2560px-Trustpilot_Logo_%282022%29.svg.png" alt="">
            </div>
          </div>

          <div class="flex flex-col w-1/2 items-start gap-2 bg-white rounded-xl p-4 lg:p-8">
            <div class="flex">
              <Icon v-for="index in 5" :key="index" icon="ic:round-star" class="w-6 h-6 text-orange-500" />
            </div>

            <div>4.1/5 <span class="text-gray-400 font-normal">(18k Reviews)</span></div>

            <div>
                <img class="w-2/3" src="https://capterra.s3.amazonaws.com/assets/images/logos/capterra.png" alt="">
            </div>
          </div>
        </div>
      </div>

      <!-- IMG (HERO) -->
      <div class="w-full lg:w-1/2 flex items-center justify-center">
        <div class="w-full h-full">
          <img class="w-full h-full bg-white rounded-2xl object-cover" src="https://cleanvid.com/_astro/woman.526ab690.png" alt="">
        </div>
      </div>
    </main>

    <!-- BANNER -->
    <div class="flex justify-between items-center gap-2 py-4 bg-gray-950 text-white md:text-lg lg:text-xl fixed left-0 right-0 bottom-0">
      <div></div>

      <div class="flex justify-between items-center gap-2">
        <div>Want to annotate? <span class="font-normal">Get Started for free</span></div>
        <button @click.prevent="" class="py-2 p-4 rounded-full bg-green-500">Sign Up</button>
      </div>
      
      <div class="px-4">
        <button click.prevent="">
          <Icon icon="mingcute:close-fill" class="w-6 h-6 text-white" />
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
