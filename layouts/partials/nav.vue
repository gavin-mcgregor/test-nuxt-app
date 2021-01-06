<template>
  <header>
      <div class="inner-header">
          <nuxt-link to="/" class="logo">LogoFile</nuxt-link>
          <nav>
            <ul>
                <li><nuxt-link to="/">About</nuxt-link></li>
                <li><nuxt-link to="/">Services</nuxt-link></li>
                <li><nuxt-link to="/">Contact</nuxt-link></li>
            </ul>
          </nav>
      </div>
      
  </header>
</template>

<script>
export default {
    
}
</script>

<style>
header {
    height: 80px;
    background-color: #333;
    display: grid;
}
.inner-header {
    align-self: center;
    max-width: 1000px;
    width: 80%;
    margin: auto;
}
.logo {
    margin-right: 40px;
    display: inline-block;
    float: left;
}
nav {
    float: right;
}
nav ul {
    list-style: none;
    padding: 0;
}
nav li {
    display: inline;
    padding: 0;
    margin-right: 1rem;
}
nav li:last-of-type {
    margin-right: 0;
}
header a {
    color: #fff;
    transition: color ease-in 0.3s;
    text-decoration: none;
}
header a:hover {
    color: #999;
}
</style>