<template>
<div>  
    <Navbar/>
    <main class="w-full p-6 bg-transparent">
      <div>
        <Nuxt />
      </div>
    
    </main>
  </div>
  
  
  </template>
  <script>
  import Navbar from '@/components/Navbar'
  export default{
    components:{
      Navbar
    }
  
  }
  </script>
  