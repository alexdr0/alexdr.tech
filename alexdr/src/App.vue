<template>
<div>
    <div id="nav-box">
      <div id="nav">
        <div class="buttons">
          <button class="button is-link is-light header-buttons">
            <router-link to="/">Home</router-link>
          </button>
          <button class="button is-link is-light header-buttons">
            <router-link to="/projects">Projects</router-link>
          </button>
        </div>
      </div>
    </div>
  <router-view/>
</div>
</template>

<style>
#nav-box{
  width:100%;
  height:40pt;
  margin-bottom:15pt;
  display:flex;
  animation-name:enter;
  animation-duration: 4s;
}
@keyframes enter{
    0%{opacity: 0;}
    75%{opacity: 0;}
    100%{opacity: 1;}
}

.header-buttons{
  font-family:Roboto Mono;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  margin: auto;
  justify-content: center;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #5589fa;
}
</style>
