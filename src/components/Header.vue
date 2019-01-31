<template>
  <div class="header">
    <header class="header">
      <img class="logo" src="@/assets/bee-logo.png" alt="logo">
      <nav class="big-nav">
        <ul class="nav-list">
          <li class="big-header">
            <a href="#">Home</a>
          </li>
          <li class="big-header">
            <a href="#">About</a>
          </li>
          <li class="big-header">
            <a href="#">Meet the squad</a>
          </li>
          <li class="hamburger"></li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style scoped lang="scss">
@import url("https://fonts.googleapis.com/css?family=Major+Mono+Display");

.header {
  position: fixed;
  width: 100%;
  background-color: black;
  color: white;
  box-shadow: 0px 0.5px 5px black;
  z-index: 2;
  font-family: "Major Mono Display", monospace;
  display: flex;
  justify-content: space-between;
}

.nav-list {
  list-style-type: none;
  display: flex;
  margin: 2.5rem 0 0 0;
  padding: 0;
  justify-content: space-around;

  a {
    color: white;
    text-decoration: none;
    font-size: 1.3rem;
  }
}

.big-header {
  margin: 0 0.5rem;
}

.logo {
  height: 3rem;
  margin: 1.5rem 0 1.5rem 0.5rem;
}

@media (max-width: 501px) {
  .big-header {
    display: none;
  }
}

@media (min-width: 600px) {
  .big-header {
    margin: 0 1.7rem;
  }
}
</style>


