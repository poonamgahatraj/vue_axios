<template>
    <h1>Hello</h1>
</template>

<script>
import vue from 'vue';
import axios from 'axios';
import vueaxios from 'vue-Axios';
vue.use(vueaxios,axios)

export default{
    data(){
        return{

        }
    },

    mounted(){
        vue.axios.get('https://api.publicapis.org/entries')
        .then((response)=>{

            console.log(response.data)
        })
    }
}
</script>