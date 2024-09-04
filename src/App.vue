<script setup>
// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'
import MyNev from './components/MyNev.vue'
import MyCard from './components/Mycard.vue'
import Noob from './components/Noob.vue'
import items from './test.json'
</script>

<template>
  <div>

    <header>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/boxicons@latest/css/boxicons.min.css">
      <MyNev />
      <h1>TheWelcome</h1>
      <div className="grid-container">
        <MyCard v-bind="items[0]" />
        <MyCard v-bind="items[1]" />
        <MyCard v-bind="items[2]" />
        <MyCard v-bind="items[3]" />
        <MyCard v-bind="items[4]" />
        <MyCard v-bind="items[5]" />
        <MyCard v-bind="items[6]" />
        <MyCard v-bind="items[7]" />
        <MyCard v-bind="items[8]" />
        <MyCard v-bind="items[9]" />
        <MyCard v-bind="items[10]" />
        <MyCard v-bind="items[11]" />
      </div>
      <footer>
      <Noob />
    </footer>
      <!-- <MyCard/> -->
      <!-- <MyCard/>
    <MyCard/> -->
      <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" /> 

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>-->
    </header>

    <main>
      <!--<TheWelcome />-->

    </main>
  </div>
</template>

<style scoped>
header {
  text-align: center;
  padding: 20px;
  background: linear-gradient(to top, rgba(0, 0, 0, 0.60)50%, rgba(0, 0, 0, 0.60)50%), url(https://img.freepik.com/free-vector/gradient-galaxy-background_52683-65386.jpg?t=st=1724818942~exp=1724822542~hmac=d82b771a154eb888230b72f50e88cefb0a579cf1cedd5dd285702d23e14cbed5&w=900);
  background-size: cover;
  background-position: center;
  animation: moveBackground 30s linear infinite;
}

@keyframes moveBackground {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 100% 100%;
  }
}

h1 {
  color: white;
  font-size: 2rem;
  margin: 0;
  padding: 10px;
}

.grid-container {
  display: grid;
  grid-column-gap: 1rem;
  grid-row-gap: 1rem;
  padding: 0 1rem;
}

footer{
  background-color: aliceblue;
}

@media (min-width: 576px) {
  .grid-container {
    grid-template-columns: repeat(1, 1fr);
  }
}

@media (min-width: 992px) {
  .grid-container {
    grid-template-columns: repeat(3, 1fr);
  }
}

/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style>