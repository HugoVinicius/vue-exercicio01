<template>
    <div class="corpo">
        <nav class="menu">
            <div class="center">
                <ul>
                    <li v-for="(element) in dados" :key="element"><a href="#">{{element}}</a></li>
                </ul>
            </div>
        </nav>
    </div>
  
</template>

<script>
export default {
    name:"NavBar",
    props:{
        dados:{
            Type: Array
        }
    }
}
</script>

<style>
.menu ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}
  
.menu li {
    float: left;
}
  
.menu  li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}  

.menu li a:hover {
    background-color: #111;
}
  
nav{
    display: flex;
    justify-content: center;
}

.corpo{
    background-color: #333;
}


</style>