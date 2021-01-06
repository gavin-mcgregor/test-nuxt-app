<template>
  <header>
    <div class="inner-header">
      <nuxt-link to="/" class="logo">Logo<span>File</span></nuxt-link>
      <Menu @clicked="navigationChange" />
      <nav :class="{ open: navigationOpen }">
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
  data() {
    return {
      navigationOpen: false
    };
  },
  methods: {
    navigationChange() {
      this.navigationOpen = !this.navigationOpen;
    }
  }
};
</script>

<style scoped>
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
  display: flex;
}
.logo {
  margin-right: 40px;
  display: inline-block;
  float: left;
  text-transform: uppercase;
  font-weight: 800;
  font-size: 1.2rem;
  line-height: 1;
  align-self: baseline;
}
.logo span {
  font-weight: normal;
}
nav {
  align-self: baseline;
  margin-left: auto;
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
.mob-menu {
  display: none;
  align-self: baseline;
  margin-left: auto;
}
@media only screen and (max-width: 640px) {
  .mob-menu {
    display: block;
  }
  nav {
    width: 0%;
    margin: 0;
    height: 100%;
    position: fixed;
    z-index: 999;
    top: 0;
    left: 0;
    background-color: #333;
    overflow-x: hidden;
  }
  nav ul {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  nav li {
    display: block;
    padding: 0.5rem 0;
  }
}
</style>
