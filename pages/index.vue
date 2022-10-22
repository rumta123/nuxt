<template>

 <div> 
    <h1>Home page</h1>
    <nuxt-link to="/about">
      About (internal link that belongs to the Nuxt App)
    </nuxt-link>

    <a href="https://nuxtjs.org">External Link to another page</a>

  </div>
  
    
    



</template>

<script>


export default {
  data() {
    return {
      title: "Home page",
    };
  },
  head() {    
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Home page description",
        },
      ],
    };
  },
};
</script>