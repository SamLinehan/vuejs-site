<template>
  <div id="app">
    <header>
      <router-link to="/" class="nameHeader"><h1>SAM LINEHAN</h1></router-link>
      <div class="betaDiv">
        <h3>Beta Website</h3>
      </div>
      <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/work">Work</router-link>
        <!--<router-link to="/resume">Resume</router-link>-->
        <router-link to="/about">About</router-link>           
      </nav>                 
    </header>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="scss">
// Variables
$header-font: 'Montserrat', sans-serif;
$main-font: 'Open Sans', sans-serif;

#app {
  display: flex;
  flex-direction: column;
  justify-content: center;  
  font-family: 'open sans';
}

header {
  width: 100%;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;

  .nameHeader {
    color: inherit;
    text-decoration: none;
    font-family: $header-font;
  }

  .betaDiv {
    h3 {
      margin-top: 0px;
    }
  }

  nav {
    a, a:visited, a:active {
      color: inherit;
      text-decoration: none;
    }

    a:hover, u {
      text-decoration: none;
    }

    width: 25%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    align-self: center;
    font-weight: 200;
  }

}
</style>
