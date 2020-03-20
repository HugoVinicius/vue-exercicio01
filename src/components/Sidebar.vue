<template>
    <div class="menuLateral">
        <ul>
             <li v-for="(element) in menuAside" :key="element"><a href="#">{{element}}</a></li>
        </ul>
    </div>  
</template>

<script>
export default {
    name:"Sidebar",
    props:{
        menuAside:{
            Type: Array
        }
    }
}
</script>

<style>
.menuLateral {
    display: flex;
    justify-content: center;
}
</style>