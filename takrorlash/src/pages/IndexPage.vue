<template >
  <div>
    <div id="app">
      <main>
        <div class="navigation">
          <header>
            <h1>Samar Badriddinov{{progres}}</h1>
          </header>
          <nav>
            <a href="#">About Us</a>
            <a href="#">Contact</a>
            <a href="#">Portifolio</a>
          </nav>
        </div>
        <CompProgresbar/>
        <CompPost />
      </main>
    </div>
  </div>
</template>
<script>
import CompPost from 'src/components/CompPost';
import CompProgresbar from '../components/CompProgresbar.vue';
export default {
  components: { CompPost, CompProgresbar },
  data() {
    return {
      process:0
    }
  },
  methods: {
      setProress(progress){
        this.progress = progress
      }
  },
}
</script>
<style >
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'monospace' sans-serif;
}

main {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  overflow: hidden;
}

.navigation {
  width: 100%;
  height: 10vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: black;
  padding: 30px;
}

header h1 {
  color: #fff;
  font-size: 32px;
}

nav a {
  margin: 0 20px;
  text-decoration: none;
  text-transform: uppercase;
  color: #fff;
}
</style>
