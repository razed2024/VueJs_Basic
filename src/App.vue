<script >
import Navbar from './components/Navbar.vue'
import AllFriends from './components/AllFriends.vue'
import OnlineFriends from './components/OnlineFriends.vue'
 export default {

  name:'App',
  data(){
    
  return{
    title:'Hurray ! Our vue apps are running',
    friends:[
            {name:'A',online:true},
            {name:'B',online:true},
            {name:'C',online:false},
            {name:'D',online:true},
            {name:'E',online:false},
        ]


  }
},
components:{
  Navbar,
  AllFriends,
  OnlineFriends,
},

methods:{
  deleteFriend(payload){
this.friends =this.friends.filter(friend =>{
 return friend.name !== payload.name
})
  }
}
 }

</script>

<template>
  <div>
  <h1 class=" text-center p-6"> {{ title }}</h1>
<Navbar/>
<AllFriends :friends="friends" @delete="deleteFriend"/>
<OnlineFriends :friends="friends" />
  </div>
  
</template>

<style scoped>

</style>
