<template>
  <div class="bg">
    <div id="app">
      <!-- <Header /> -->
      <!-- <Analytics /> -->
      <div id="content">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
};
</script>

<style>
:root {
  --text-color: #0ebe08;
  --link-color: #be3c08;
  --hover-color: #ffffff;
  font-size: 150%;
}

body,
html {
  height: 100%;
  background-color: white;
  margin: 0;
}

#app {
  font-family: Georgia, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--text-color);
}

#content {
  max-width: 70ch;
  padding: 2ch;
  margin: auto;
}

@media screen and (max-width: 600px) {
  .bg {
    background-size: auto;
  }
}

a {
  color: var(--link-color);
  font-weight: bold;
}
a.active {
  color: var(--link-color);
}
a:hover {
  color: var(--hover-color);
}

img {
  max-width: 100%;
  height: auto;
}

hr {
  width: 50%;
  border-color: var(--text-color);
}

span.title {
  font-style: italic;
}

button {
  background-color: #410000;
  color: var(--text-color);
  font-size: 18px;
  text-align: center;
  border-radius: 5px;
  border: 2px solid var(--text-color);
  padding: 10px 25px;
  margin: 0px 15px;
  font-family: Georgia, serif;
  cursor: pointer;
  outline: none;
  opacity: 0.8;
  transition: 0.3s;
}
button:hover {
  opacity: 1;
  background-color: #6a0000;
}
</style>
