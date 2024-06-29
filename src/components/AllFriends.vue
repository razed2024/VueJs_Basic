<script>
export default {
name:'AllFriends',
props:['friends'],
data(){
    return{
      
    }

},
methods:{
    unfriend(name){
        this.$emit('delete',{name})
    }
}
}

</script>


<template>
    <div id="allFriends">
        <h2 class=" text-center"> All Friends</h2>
        <div v-for=" (friend, index) in friends" :key="index" class=" text-center">
            <h4 @click="unfriend(friend.name)">{{ friend.name}}</h4> 

        </div>
      
    </div>
</template>


<style>


</style>