<template>

  <app-header v-bind:title="name"></app-header>

  <app-article v-bind:users="users"></app-article>

  <app-footer v-bind:title="title"></app-footer>

</template>

<script>
import Header from "./components/header.vue"
import Footer from "./components/footer.vue"
import Article from './components/article.vue'

export default {
  components:{
    "app-header":Header,
    "app-footer":Footer,
    "app-article":Article,
  },
  data(){
    return{
      name:"Anasayfa",
      title:"Budotekno",
      users:[
                { name:"Buğra", job:"Geliştirici",status:false},
                { name:"Ali", job:"Geliştirici",status:false},
                { name:"Veli", job:"Geliştirici",status:false},
                { name:"Hasan", job:"Geliştirici",status:false},
                { name:"Mehmet", job:"Geliştirici",status:false},
                { name:"Fatma", job:"Geliştirici",status:false},
            ]
    }
  },
 
  
}
</script>
