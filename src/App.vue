<template>
  <div id="app">
    <header>
      <nav
        class="navbar fixed-top navbar-light"
        style="background-color: pink"
      >
        <h2 class="text-dark h2">
          <a class="navbar-brand" href="#" >
            <img
              src="https://yt3.ggpht.com/ytc/AAUvwnhTEa6kEyqgSvL3wMaMbUDZtyHvhXehJppDCeOGUCI=s900-c-k-c0x00ffffff-no-rj"
              width="75"
              height="75"
              alt=""
              loading="lazy"
            /> </a
          >Pink Panther, Information
          
        </h2>
      </nav>
    </header><br>
    <Axios />
    <footer>
      <nav class="navbar navbar-light" style="background-color: pink">
        <h2 class="text-dark h2">
          <a class="navbar-brand" href="https://www.nasa.gov/" target="_blank"> 
            <img
              src="https://lh3.googleusercontent.com/-9SbvMHKLu_o/UdPLXZmCFWI/AAAAAAAAB1E/ncgeI6ECwvE/s400/NASA-logo_53.jpg"
              width="60"
              height="50"
              alt=""
              loading="lazy"
            />
          </a>
        </h2>
      </nav>
    </footer>
  </div>
</template>

<script>
import Axios from "./components/axios.vue";
export default {
  name: "App",
  components: {
    Axios,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: auto;
  height: auto;
  background-image: url("https://c4.wallpaperflare.com/wallpaper/368/774/419/pink-panther-wallpaper-preview.jpg");
  margin-top: 100px;
  border-radius: 10px;
}
header {
  margin-bottom: 15vh;
}
footer {
  margin-top: 15vh;
  background-image: url("https://images.unsplash.com/photo-1451187580459-43490279c0fa?ixid=MXwxMjA3fDB8MHxzZWFyY2h8MXx8bmFzYXxlbnwwfHwwfA%3D%3D&ixlib=rb-1.2.1&w=1000&q=80");
  
}
</style>