<template>


<div >
      <h1>{{ title }}</h1>
</div>


</template>
<script >
export default {
 
  data() {

   
    return {
      
      title:"Обо мне",
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