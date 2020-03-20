<template>
  <div id="app">
    <Header :dados="dadosSite.menuTop"/>
    <NavBar :dados="dadosSite.menuPrincipal"/>
    <Content :dados="dadosSite"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import NavBar from './components/NavBar.vue'
import Content from './components/Content'

export default {
  name: 'App',
  components: {
    Header,
    NavBar,
    Content
  },
  data(){
    return{
      dadosSite: {
          menuTop: ['Topic 1', 'Topic 2', 'Topic 3', 'Topic 4'],
          menuPrincipal: ['Main menu 1', 'Main menu 2', 'Main menu 3'],
          menuAsideLink: ['Section 1', 'Section 2', 'Section 3', 'Section 4', 'Section 5',
            'Section 6', 'Section 7', 'Section 8', 'Section 9', 'Section 10',
            'Section 11', 'Section 12', 'Section 13', 'Section 14', 'Section 15'],
          Materias: [
            {
              nome: "Matéria 1",
              conteudo: "Matéria 1. Veritatis doloribus doloremque ab qui culpa dignissimos explicabo natus optio omnis incidunt recusandae, perferendis dicta, animi ad. Aliquam nostrum sequi inventore vero! (...)"
            },
            {
              nome: "Matéria 2",
              conteudo: "Matéria 2. Veritatis doloribus doloremque ab qui culpa dignissimos explicabo natus optio omnis incidunt recusandae, perferendis dicta, animi ad. Aliquam nostrum sequi inventore vero! (...)"
            },
            {
              nome: "Matéria 3",
              conteudo: "Matéria 3. Veritatis doloribus doloremque ab qui culpa dignissimos explicabo natus optio omnis incidunt recusandae, perferendis dicta, animi ad. Aliquam nostrum sequi inventore vero! (...)"
            },
            {
              nome: "Matéria 4",
              conteudo: "Matéria 4. Veritatis doloribus doloremque ab qui culpa dignissimos explicabo natus optio omnis incidunt recusandae, perferendis dicta, animi ad. Aliquam nostrum sequi inventore vero! (...)"
            },
            {
              nome: "Matéria 5",
              conteudo: "Matéria 5. Veritatis doloribus doloremque ab qui culpa dignissimos explicabo natus optio omnis incidunt recusandae, perferendis dicta, animi ad. Aliquam nostrum sequi inventore vero! (...)"
            }
          ]
      }
    }
  }
}
</script>

<style>
*{
	margin: 0;
	padding: 0;
	border: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.App {
  text-align: center;
}

.App-logo {
  animation: App-logo-spin infinite 20s linear;
  height: 40vmin;
  pointer-events: none;
}

.App-header {
  background-color: #282c34;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-size: calc(10px + 2vmin);
  color: white;
}

.App-link {
  color: #61dafb;
}
</style>
