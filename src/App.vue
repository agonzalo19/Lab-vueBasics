<template>
<div id="app">
  <NavBar />
  <div class="divSuma" >
    {{resultSuma()}}
    </div>
    <h1 v-if="show">Vue is awesome!</h1>
    <button @click="show=true">Click</button>

    <p v-for="element in grocerias" :key="element">{{element.name}}</p>
  <Footer />
</div>
</template>


<script>
import NavBar from './components/NavBar.vue'
import Footer from './components/Footer.vue'

export default ({
  data() {
    return{
      show: false,
      grocerias: [{name: "Tomate"}, {name: "Lechuga"}],
    }
},
//     methods() {
//     resultSuma()
//     return {2+2},
//     }
// }

components: {
      NavBar,
      Footer,
},

})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.divSuma{
  display: flex;
  border: solid red 4px;
  justify-content: center;
}
</style>
