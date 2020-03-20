<template>
    <header class="header">
        <div class="headerTopo">
            <img src="../assets/logo.png" alt="logo" width="200px" />
            <ul class="headerMenu">
                <li v-for="(element) in dados" :key="element"><a href="#">{{element}}</a> </li>            
            </ul>
        </div>
        <div class="headerFooter">
            <input class="inputPesquisa" type="text" placeholder="Search" aria-label="Search"/>
        </div>
    </header>
</template>

<script>
export default {
    name:"Header",
    props:{
        dados:{
            Type: Array
        }
    }
}
</script>

<style>
.header ul, li, p{
    margin: 0px;
    padding: 0px;
    list-style: none;
    font-size: 1.2rem;
    font-family: Arial, Helvetica, sans-serif;
}

.header a{
    text-decoration: none;
}

.headerTopo{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
    padding: 10px;
    flex-wrap: wrap;
}

.headerMenu{
    display: flex;
}

.headerMenu li{
    margin-left: 10px;
}

.headerMenu li a{
    display: block;
    padding: 10px;
    color: black;
}

.headerMenu li a:hover {
    background-color: #111;
    color: white;
}

.headerFooter{
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    margin-top: -60px;
    margin-right: 10px;
    padding: 10px;
}

.inputPesquisa{
    padding-left:35px;
	padding-top:6px;
	height:30px;
	background-image:url(../assets/lupa.jpg);
    background-repeat:no-repeat;
    font-size: 1.2rem;
    font-family: Arial, Helvetica, sans-serif;    
}

@media screen and (max-width: 630px){
    .headerFooter {
        display: none;      
    }
}
</style>