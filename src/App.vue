<template>
  <nav class="header">
    <ul class="nav">
      <li><router-link to="/" id="home">Home</router-link></li>
      <li><router-link to="/addPost">Add Post</router-link></li>
      <li><router-link to="/signup">Signup</router-link></li>
      
    </ul>

    <div class="user-profile">
        <a id="logo" class="logo" href="#"><img src="me.jpg" width="60" height="60" alt="My picture" id="user-photo"></a>
        <div class="dropdown" id="dropdown">
          <ul>
            <li><a href="#">John Doe</a></li>
            <li><a href="#">john.doe@ut.ee</a></li>
            <li><a href="#">logout</a></li>
          </ul>
        </div>
    </div>
  </nav>
  <router-view/>
</template>



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

.logo .post-logo {
    margin: 0;
    font-size: 1.1em;
}

.logo {
    margin-right: 10px;
}

.user-profile {
  margin-left:auto;
}
</style>
<script setup>
</script>