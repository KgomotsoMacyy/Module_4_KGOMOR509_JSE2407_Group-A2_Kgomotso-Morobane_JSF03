<script setup>
import { RouterLink, RouterView } from 'vue-router'
import ProductList from './components/ProductList'
</script>

<template>
  <header class="bg-white">
    <div class="wrapper">
      <nav class="flex justify-between items-center w-[92%] mx-auto">
        <router-link to="/">
          <div>
            <img class="w-16" src="../public/favicon.ico" alt="logo">
          </div>
        </router-link>
        <div class="md:static absolute text-2xl text-black md:min-h-fit min-h-[60vh] left-0 top-[-100%] md:w-auto w-full flex items-center px-5 ">
          <ul class="flex md:flex-row flex-col md:items-center md:gap-[4vw] gap-8">
            <li>
              <router-link to="/">TakeItAll</router-link>
            </li>
          </ul>
        </div>
        <div>
          <button class="flex items-center px-3 py-3 hover:bg-gray-200">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16">
              <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"/>
            </svg>
          </button>
        </div>
      </nav>
    </div>
  </header>

  <template>
    <div id="app">
      <ProductList />
    </div>
  </template>
</template>


<style scoped>

</style>
