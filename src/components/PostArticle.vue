<template>
    <article class="notica">
        <img src="../assets/noticia.jpg" alt="Imagem da noticia em questão" />
        <div>
            <p> {{materia.conteudo}} </p>
        </div>
    </article>
</template>

<script>
export default {
    name:"PostArticle",
    props:{
        materia:{
            Type: Object
        }
    }
}
</script>

<style>

</style>