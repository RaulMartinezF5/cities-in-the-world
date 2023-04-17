<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header/Header.vue';

</script>

<template>
  
  <Header></Header>
  <RouterView />
  <footer>
    <h5>© Company, inc 2021</h5>
    <div class="icons"><img src="./assets/icons.png" alt="icons"></div>
  </footer>
</template>

<style lang="scss" scoped>
@use '../src/assets/main' as *;
  
  footer{
    @include FlexDisplay(row, flex-start, center, 100%, auto);
    border-top: 1px solid;
    h5{
      padding: 2%;

    }
    .icons{
      display: flex;
      align-items: center;
      justify-content: flex-end;
      margin-left: auto;
      margin-right: 50xp;
    }

  }
</style>
