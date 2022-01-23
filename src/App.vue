<script setup></script>

<template>
  <div class="wrapper">
    <main class="main container">
      <router-view />
    </main>
  </div>
</template>

<style>
  :root {
    --background-color: #fff;
  }

  * {
    margin: 0;
    padding: 0;
    list-style: none;
    text-decoration: none;
    box-sizing: border-box;
  }

  body {
    background-color: var(--background-color);
    color: #333;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 16px;
  }

  .container {
    width: 85%;
    margin: 0 auto;
  }

  .wrapper {
    display: grid;
    grid-template-areas:
      'navbar'
      'main';
    grid-template-rows: 3rem 1fr;
    grid-template-columns: 1fr;
    height: 100vh;
  }

  .card {
    background-color: rgb(7, 114, 185);
    border-radius: 0.5rem;
    padding: 1rem;
    color: #fff;
  }

  .main {
    grid-area: main;
    overflow: auto;
  }
</style>
