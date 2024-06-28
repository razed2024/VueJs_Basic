<script>
export default {
name:'Navbar',
data(){
    return{

    }

}
}

</script>


<template>
    <div>
        <nav>
            <ul class="">
                 <li> <a href=""> Home </a></li>
                 <li> <a href=""> Post </a></li>
                 <li> <a href=""> About </a></li>
                 <li> <a href=""> Contact </a></li>
            </ul>
        </nav>
    </div>
</template>


<style scoped>
nav{
    text-align: center;
}
nav ul{
    padding: 0;
}
nav li{
    display: inline-block;
    list-style-type: none;
    margin:0;
   
}

</style>