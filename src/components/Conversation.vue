<script setup lang="ts">
import { NCard, NTag, NButton, NInput } from "naive-ui";
</script>

<template>
        <div class="container">
          <NCard hoverable>
            <template #cover><NTag type="info">Furious</NTag></template><br>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
          </NCard>
        </div>
        <div class="container">
          <NCard hoverable embedded>
            <template #cover><NTag type="error">In-Alt</NTag></template><br>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
          </NCard>
        </div>
        <div class="container">
          <NCard hoverable>
            <template #cover><NTag type="info">Furious</NTag></template><br>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
          </NCard>
        </div>
        <div class="container">
          <NInput type="textarea" rows=10 placeholder="Reply to conversation"></NInput>
          <br /><br />
          <NButton type="info">Reply</NButton>
        </div>
</template>

<style>
@import "@/assets/base.css";

* {
  margin: 0;
  padding: 0;
}

#app {
  max-width: 10000px;
  /*margin: 0 auto;
  padding: 2rem;

  font-weight: normal;*/
}

header {
  padding: 0;
  margin: 0;
  line-height: 1.5;
  /*max-height: 100vh;*/
}

.container {
  padding: 20px;
  width: 100%;
}

.flex-layout {
  display: flex;
  flex-direction: row;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

a,
.green {
  text-decoration: none;
  color: hsla(160, 100%, 37%, 1);
  transition: 0.4s;
}

@media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  body {
    padding: 0;
    margin: 0;
    /*display: flex;*/
    /*place-items: center;*/
  }

  #app {
    display: grid;
    grid-template-columns: 1fr;
    padding: 0 2rem;
  }

  .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
    padding: 0 20%;
    border-left: solid lightgray 1px;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  nav {
    text-align: right;
    /*margin-left: -1rem;*/
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
