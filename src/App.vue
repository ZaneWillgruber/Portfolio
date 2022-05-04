<template>
  <div>
  <NavigationBar/>
  <router-view />
  </div>
</template>

<script>
import NavigationBar from "./components/NavigationBar"

export default {
  name: 'App',
  components: {
    NavigationBar,
  },
  data() {
    return {
      title: 'Zane Willgruber Portfolio'
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@400;500&display=swap');
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Raleway", sans-serif;
  font-weight: 400;
}
.app {
  min-height: 100vh;
  position: relative;
  background-color: #f1f1f1;
}
.container {
  padding: 0 20px;
  max-width: 1140px;
  margin: 0 auto;
}
</style>
