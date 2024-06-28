<script>
export default {
name:'OnlineFriends',
props:['friends'],
data(){
    return{
        
    }

}
}

</script>


<template>
    <div id="onlineFriends">
        <h2 class=" text-center">Online Friends</h2>
            
            <div v-for=" (friend, index) in friends" :key="index" class=" text-center">
                <h6 v-if="friend.online"> {{ friend.name }}</h6>
        
            </div>
       
    </div>
</template>


<style scoped>

</style>