<template>
    <section >
      <div v-if="$route.query.message" class="w-full max-w-xs  ">
        <div class="shadow-lg bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 pl-1.5"> <p>Нужно ввести логин</p></div>
       
      </div>
        <div class="w-full max-w-xs">
  <form class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4" @submit.prevent="onSubmit">
    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="username">
        Username
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="username" type="text" placeholder="Username">
    </div>
    <div class="mb-6">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="password">
        Password
      </label>
      <input class="shadow appearance-none border border-red-500 rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline" id="password" type="password" placeholder="******************">
      <p class="text-red-500 text-xs italic">Please choose a password.</p>
    </div>
    <div class="flex items-center justify-between">
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="submit" >
        Sign In
      </button>
      <a class="inline-block align-baseline font-bold text-sm text-blue-500 hover:text-blue-800" href="#">
        Forgot Password?
      </a>
    </div>
  </form>
  <p class="text-center text-gray-500 text-xs">
    &copy;2020 Acme Corp. All rights reserved.
  </p>

  <nuxt-link to="/">Назад</nuxt-link>
</div>
    </section>
</template>

<style scoped>
.my{
    margin: 0 auto;
}
</style>

<script>
export default{
    layout:'empty',
    methods:{
      onSubmit(){
        this.$store.dispatch('login')
        this.$router.push('/')
      }
    }
}
</script>