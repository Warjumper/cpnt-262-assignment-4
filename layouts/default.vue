<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4 flex justify-between">
        <NuxtLink to="/" class="font-bold">Assignment 4</NuxtLink>
        <ul class="flex gap-4">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/contact">Contact</NuxtLink></li>
          <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
          <li><NuxtLink to="/products/error" class="btnTwo">Error Page</NuxtLink></li>
        </ul> 
      </nav>
    </header>

    <!-- output page content -->
    <div class="container mx-auto p-4">
      <slot />
    </div>
  </div>



  <footer class="shadow-sm bg-black text-white fixed bottom-0 left-0 w-screen">
    <div class="flex justify-around space-x-32 py-10">
        <ul class="flex gap-4">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/contact">Contact</NuxtLink></li>
          <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
        </ul>
        <div class="text-white">Copyright &copy; 2022, Jesse H</div>
    </div>  
  </footer>
</template>

<style scoped>
  .router-link-exact-active {
    color: rgb(125, 123, 247);
  }
</style>