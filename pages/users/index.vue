<template>
    <section>
        <h1>Users pages</h1>
        <ul>
            <li v-for="user of 5" :key="user"> 
             <a href="#" @click.prevent="openUser(user)"> user {{user}}</a>  
            </li>
        </ul>
    </section>
    
</template>

<script>
export default{
    methods:{
        openUser(user){
            this.$router.push('/users/'+ user)
        }
    }
}
</script>