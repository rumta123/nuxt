<template>


  <div>
    <h1>{{ title }}</h1>

    <div class="relative overflow-hidden bg-white">
      <div class="mx-auto max-w-7xl">
        <div class="relative z-10 bg-white pb-8 sm:pb-16 md:pb-20 lg:w-full lg:max-w-2xl lg:pb-28 xl:pb-32">
          <svg class="absolute inset-y-0 right-0 hidden h-full w-48 translate-x-1/2 transform text-white lg:block"
            fill="currentColor" viewBox="0 0 100 100" preserveAspectRatio="none" aria-hidden="true">
            <polygon points="50,0 100,0 50,100 0,100" />
          </svg>

          <div>
            <div class="relative px-4 pt-6 sm:px-6 lg:px-8">

            </div>

            <!--
            Mobile menu, show/hide based on menu open state.
  
            Entering: "duration-150 ease-out"
              From: "opacity-0 scale-95"
              To: "opacity-100 scale-100"
            Leaving: "duration-100 ease-in"
              From: "opacity-100 scale-100"
              To: "opacity-0 scale-95"
          -->

          </div>

          <main class="mx-auto mt-10 max-w-7xl px-4 sm:mt-12 sm:px-6 md:mt-16 lg:mt-20 lg:px-8 xl:mt-28">
            <div class="sm:text-center lg:text-left">
              <h1 class="text-4xl font-bold tracking-tight text-gray-900 sm:text-5xl md:text-6xl">
                <span class="block xl:inline">Евгений Румянцев</span>
                <span class="block text-indigo-600 xl:inline">vue+nuxt.js</span>
              </h1>
              <p
                class="mt-3 text-base text-gray-500 sm:mx-auto sm:mt-5 sm:max-w-xl sm:text-lg md:mt-5 md:text-xl lg:mx-0">
                Занимаюсь профессиональной разработкой сайтов и приложений </p>
              <p
                class="mt-3 text-base text-gray-500 sm:mx-auto sm:mt-5 sm:max-w-xl sm:text-lg md:mt-5 md:text-xl lg:mx-0">
                Отзывы </p>
              <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                  <a href="https://youdo.com/u5621184"
                    class="flex w-full items-center justify-center rounded-md border border-transparent bg-indigo-600 px-8 py-3 text-base font-medium text-white hover:bg-indigo-700 md:py-4 md:px-10 md:text-lg">youdo</a>
                </div>
                <div class="mt-3 sm:mt-0 sm:ml-3">
                  <a href="https://vk.com/rum44"
                    class="flex w-full items-center justify-center rounded-md border border-transparent bg-indigo-100 px-8 py-3 text-base font-medium text-indigo-700 hover:bg-indigo-200 md:py-4 md:px-10 md:text-lg">Vk</a>
                </div>
              </div>
            </div>
          </main>
        </div>
      </div>
      <div class="lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
        <img class="h-56 w-full object-cover sm:h-72 md:h-96 lg:h-full lg:w-full"
          src="https://sun1-87.userapi.com/impf/O31IBThvOqey0ENTydlHiHXwBHMIU-fp074ESA/WHLPFP60t64.jpg?size=1024x1024&quality=96&sign=0afa72ccf1cffe0e5eacab2b78d6937c&type=album"
          alt="">
      </div>
    </div>


  </div>


</template>
<script >
export default {

  data() {


    return {

      title: "Главная страница",
    };
  },
  head: {
    title: 'my website title',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },
      {
        hid: 'description',
        name: 'description',
        content: 'Главная страница сделаная на nuxt 3'
      }
    ],
    link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }]
  }
};
</script>
<style>
.ease-in-out {
  width: 100vw;
}
</style>
<style scoped>
.h-56 {
  height: 100%;
}
</style>
