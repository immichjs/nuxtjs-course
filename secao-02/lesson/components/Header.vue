<template>
  <header class="flex items-center justify-between h-20 border-b bg-white shadow-sm px-16">
    <NuxtLogo class="w-12"/>
    <ul class="flex gap-2 text-xl font-semibold text-trueGray-700">
      <li class="py-4 px-6 hover:bg-trueGray-200 rounded transition duration-300">
        <NuxtLink to="/">Home</NuxtLink>
      </li>
      <li class="py-4 px-6 hover:bg-trueGray-200 rounded transition duration-300">
        <NuxtLink to="/users">Users</NuxtLink>
      </li>
      <li class="py-4 px-6 hover:bg-trueGray-200 rounded transition duration-300">
        <NuxtLink to="/products">Products</NuxtLink>
      </li>
    </ul>
  </header>
</template>
