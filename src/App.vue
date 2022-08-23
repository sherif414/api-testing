<template>
  <main>
    <!-- first section -->

    <section
      class="bg-#F6EBDA grid lg:grid-rows-[min-content_1fr] items-center min-h-screen text-center lg:text-left lg:px-10rem">

      <!-- navbar -->

      <nav class=" hidden md:flex text-black justify-between items-center py-2rem">
        <a href="#">
          <img src="/src/assets/logo.svg" alt="logo">
        </a>
        <ul class="flex gap-2rem">
          <a href="#" class="text-primary">About us</a>
          <a href="#">Our Products</a>
          <a href="#">Delivery</a>
        </ul>
        <div class="relative flex gap-1rem items-center">
          <span class="i-akar-icons-search absolute left-10px top-25% text-surface" />
          <input class="pl-2.5rem pr-1rem text-sm py-2 rounded-1rem focus:outline-none shadow"
            type="search" placeholder="search">
          <div class="i-akar-icons-cart hover:cursor-pointer " />
        </div>
      </nav>

      <!-- body -->

      <div class="grid lg:grid-cols-2 justify-items-center gap-8 lg:grid-rows-1 lg:items-center">
        <img class="lg:hidden" src="./assets/logo.svg" alt="logo">
        <div class="flex flex-col px-2rem lg:px-0">
          <h1 class="lg:text-5xl text-2xl lg:w-16ch font-semibold text-secondary lg:leading-[1.3]">
            enjoy your <span class="text-primary">coffee</span> before your activity
          </h1>
          <p class="text-gray text-sm lg:w-40ch mb-2rem">
            Boost your productivity and build your mood with a glass of coffee in the morning
          </p>
          <div class="flex justify-center lg:justify-start">
            <button
              class=" pl-4 pr-1 py-1 rounded-2rem bg-secondary text-white flex gap-0.5rem items-center">order
              now
              <div class="rounded-50% bg-primary p-2">
                <div class="i-akar-icons-cart text-white" />
              </div>
            </button>
            <button class="text-primary ml-2rem lg:inline hidden">learn more</button>
          </div>
        </div>
        <img
          class="lg:scale-80 2xl:scale-120 scale-70 xl:scale-100 p-0 m-0 lg:relative lg:left-5rem"
          src="/src/assets/coffeemog.svg" alt="coffee mog">
      </div>
    </section>

    <!-- second section -->

    <section class="lg:px-10rem px-2rem bg-white pt-5rem mb-20rem text-black">
      <h2 class="text-xl mb-8 font-bold">
        Popluar <span class="underline-primary underline underline-3px">now</span>
      </h2>
      <div class="grid lg:grid-cols-3 grid-cols-1 gap-4">
        <CardPopular heading="vanilla latte" :rating="4.5">
          <img class="w-full" src="/src/assets/coffeemog1.png" alt="heading">
        </CardPopular>
        <CardPopular heading="espresso" :rating="4.8">
          <img class="w-full" src="/src/assets/coffeemog2.png" alt="heading">
        </CardPopular>
        <CardPopular heading="hazelnut latte" :rating="4.6">
          <img class="w-full" src="/src/assets/coffeemog3.png" alt="heading">
        </CardPopular>
        <CardPopular heading="hot milk" :rating="4.7">
          <img class="w-full" src="/src/assets/coffeemog4.png" alt="heading">
        </CardPopular>
        <CardPopular heading="cappucino" :rating="4.4">
          <img class="w-full" src="/src/assets/coffeemog5.png" alt="heading">
        </CardPopular>
        <CardPopular heading="coffee ice cream" :rating="4.3">
          <img class="w-full" src="/src/assets/coffeemog6.png" alt="heading">
        </CardPopular>

      </div>

      <h2 class="text-xl mb-16 mt-40 font-bold">
        How to use our delivery <span
          class="underline-primary underline underline-3px">service</span>
      </h2>
      <div class="grid lg:grid-cols-3 justify-items-center font-bold text-lg gap-8 lg:gap-4">
        <div><img class="mb-4" src="/src/assets/service1.svg" alt="svg devlivary serivce steps">
          <h3>order your coffee</h3>
          <p class="font-normal text-sm text-gray text-center">over 20+ kinds of coffees</p>
        </div>
        <div><img class="mb-4" src="/src/assets/service2.svg" alt="svg devlivary serivce steps">
          <h3>we deliver it to you</h3>
          <p class="font-normal text-sm text-gray text-center">5 mins Delivery</p>
        </div>
        <div>
          <img class="mb-4" src="/src/assets/service3.svg" alt="svg devlivary serivce steps">
          <h3>enjoy your coffee</h3>
          <p class="font-normal text-sm text-gray text-center">hot and delicious</p>
        </div>
      </div>
    </section>

    <!-- section three -->

    <section
      class="bg-coffee text-center lg:text-left grid justify-items-center gap-8 lg:grid-cols-2 lg:pb-0 pb-8 text-black px-2rem lg:px-10rem">
      <img class="relative bottom-5rem border-4 border-white rounded-md shadow-lg"
        src="/src/assets/about_coffee.png" alt="coffee mog">
      <div class="flex flex-col justify-center items-center lg:items-start gap-8">
        <h2 class="text-3xl font-bold">
          About <span class="underline-primary underline underline-3px">us</span>
        </h2>
        <h3 class="text-xl font-bold">
          We provide quality coffee, and ready to deliver.
        </h3>
        <p class="leading-snug text-gray">
          We are a company that makes and distributes delicious drinks. our main product is made
          with a secret recipe and available in stores worldwide.
        </p>
        <button class="px-4 text-xs py-2 rounded-2rem w-max bg-secondary text-surface">Get
          your
          coffee</button>
      </div>
    </section>

    <!-- section four -->

    <section>
      <TestmonialSec />
    </section>
  </main>
</template>
<script lang="ts" setup>
import CardPopular from './components/CardPopular.vue';
import TestmonialSec from './components/TestmonialSec.vue';
</script>
<style>
html {
  background: #fff;
}

.bg-coffee {
  background-image: url('/src/assets/bg.svg');
}
</style>
