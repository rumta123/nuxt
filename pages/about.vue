

<template>
  <div class="max-w-md mx-auto bg-white rounded-xl shadow-md overflow-hidden md:max-w-2xl">
    <div class="md:flex">
      <div class="md:shrink-0">
        <img class="h-48 w-full object-cover md:h-full md:w-48"
         src="https://sun1-87.userapi.com/impf/O31IBThvOqey0ENTydlHiHXwBHMIU-fp074ESA/WHLPFP60t64.jpg?size=1024x1024&quality=96&sign=0afa72ccf1cffe0e5eacab2b78d6937c&type=album" alt="Modern building architecture">
      </div>
      <div class="p-8">
        <div class="uppercase tracking-wide text-sm text-indigo-500 font-semibold">профессиональная вебразработка</div>
        <p class="mt-2 text-slate-500">js, jq, vue.js + nuxt.js, php </p>
        <p class="mt-2 text-slate-500">wordpress, modx, opencart</p>
       <p class="mt-2 text-slate-500">Контакты для связи</p>
        <ul>
           <li v-for="link in links" :key="link.service">
           {{link.service }} - <a class=" mt-1 text-lg leading-tight font-medium text-black hover:underline" :href="link.href">{{ link.href}} </a> 
          </li>
        </ul>
       
      </div>
    </div>
  </div>
  
  
  
    
      
      
  
  
  
  </template>
  
  <script>
  
  
  export default {
    data() {
      return {
        title: "Контакты",
        links:[{'service':'youdo',  'href':'https://youdo.com/u5621184'},{'service':'telegram','href':'https://t.me/Roger_ver'} ,{'service':'github','href':'https://github.com/rumta123'}, {'service':'watsapp', 'href':'https://wa.me/79206403828'}  ],
        wordpres:[{'type':'визитка для психолога','href':'https://ovsyannikova.pro/'}],
        opencart:[{'type':'интернет магазин штор', 'href':'shtory-optom.com'}],
        modx:[{'type':'сайт для потолка', 'href':'https://dinopotolok.ru/'}]
      };
    },
    head() {    
      return {
        title: this.title,
        meta: [
          {
            hid: "description",
            name: "description",
            content: "Контакты ",
          },
        ],
      };
    },
  };
  </script>