<template>
  <main-layout>
    <div class=content>
      <img alt="Varghand logo" class="logo" src="../assets/varghand.png">
      <h1>Our games:</h1>
      <a href="https://www.sound-realms.com"><img src="../assets/dreadhorn.png" class="logo" /></a>
    </div>
  </main-layout>
</template>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}


.logo {
  padding: 12px;
  max-width: 90%;
  height: auto;
  object-fit: scale-down;
}
</style>
