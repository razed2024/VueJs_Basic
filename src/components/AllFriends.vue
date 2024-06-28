<script>
export default {
name:'AllFriends',
props:['friends'],
data(){
    return{
      
    }

}
}

</script>


<template>
    <div id="allFriends">
        <h2 class=" text-center"> All Friends</h2>
        <div v-for=" (friend, index) in friends" :key="index" class=" text-center">
            <span f-if="friend.online"> {{ friend.name}}</span>

        </div>
      
    </div>
</template>


<style>


</style>