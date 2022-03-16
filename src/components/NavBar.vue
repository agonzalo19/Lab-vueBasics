<template>
  <div>
    <nav>
      <router-link class="menu-link" to="/">Home</router-link> |
      <router-link class="menu-link" to="/about">About</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
nav{
    display: flex;
    text-align: center;
    justify-content: center;
    background-color: aquamarine;
    padding: 20px;

}

.menu-link{
    margin: 5px;
}
</style>