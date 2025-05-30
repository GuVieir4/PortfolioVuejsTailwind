<template>
  <nav class="navegacao bg-gray-900 w-full z-[1] p-8">
    <ul class="menu flex justify-center list-none gap-10">
      <li>
        <router-link to="/" class="menulink no-underline text-gray-100 font-medium relative p-1 
          after:content-[''] after:h-1 after:w-0 after:absolute after:bottom-0 after:left-0 
          after:bg-blue-500 after:transition-all after:duration-300 hover:after:w-full">
          Início
        </router-link>
      </li>
      <li>
        <router-link to="/about" class="menulink no-underline text-gray-100 font-medium relative p-1 
          after:content-[''] after:h-1 after:w-0 after:absolute after:bottom-0 after:left-0 
          after:bg-blue-500 after:transition-all after:duration-300 hover:after:w-full">
          Sobre
        </router-link>
      </li>
      <li>
        <router-link to="/contact" class="menulink no-underline text-gray-100 font-medium relative p-1 
          after:content-[''] after:h-1 after:w-0 after:absolute after:bottom-0 after:left-0 
          after:bg-blue-500 after:transition-all after:duration-300 hover:after:w-full">
          Contato
        </router-link>
      </li>
    </ul>
  </nav>
</template>
