<script lang="ts">
	import '../app.css';
	import { onMount } from 'svelte';
	
	
	let isDark = false;
	
	onMount(() => {
	  const storedDark = localStorage.getItem('theme') === 'dark';
	  isDark = storedDark;
  
	  const isSystemDarkMode = window.matchMedia('(prefers-color-scheme: dark)').matches;
	  isDark = isSystemDarkMode || isDark; 
	  document.documentElement.classList.toggle('dark', isDark);
  
	  window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', (e) => {
		isDark = e.matches;
		document.documentElement.classList.toggle('dark', isDark);
	  });
	});
	
	function toggleDarkMode() {
	  isDark = !isDark;
	  document.documentElement.classList.toggle('dark', isDark);
	  localStorage.setItem('theme', isDark ? 'dark' : 'light');
	}
  
	let { children } = $props();
  </script>
  
  <style type="text/tailwindcss"></style>
  
  {@render children()}
  
  <nav class="fixed top-4 inset-x-0 z-50">
	<div class="mx-4 max-w-screen-xl px-6 py-2 bg-white/85 dark:bg-gray-900/85 backdrop-blur shadow-lg rounded-full flex items-center justify-between transition-all duration-300 ease-in-out">
	  <!-- Logo -->
	  <a href="./" class="flex items-center">
		<img src="assets/image/logo glint.png" alt="Logo" class="h-14 w-14 object-contain transition-transform hover:scale-110">
	  </a>
  
	  <!-- Desktop Navigation -->
	  <div class="hidden lg:flex items-center space-x-6 text-gray-900 dark:text-white text-lg font-medium">
		<a href="./" class="hover:text-blue-500 transition">Home</a>
  
		<!-- Products Dropdown -->
		<div class="relative group">
		  <a href="product" class="flex items-center cursor-pointer hover:text-blue-500 transition">
			<span>Products</span>
			<svg class="ml-1 w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
			  <path d="M19 9l-7 7-7-7" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
			</svg>
		  </a>
		  <div class="absolute left-0 mt-2 w-48 bg-white/90 dark:bg-gray-900/90 shadow-md rounded-md opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-300 ease-out">
			<a href="tshirt" class="block px-4 py-2 hover:bg-gray-400 dark:hover:bg-gray-400">T-shirt</a>
			<a href="jacket" class="block px-4 py-2 hover:bg-gray-400 dark:hover:bg-gray-400">Jacket</a>
			<a href="shirts" class="block px-4 py-2 hover:bg-gray-400 dark:hover:bg-gray-400">Shirt</a>
		  </div>
		</div>
  
		<a href="services" class="hover:text-blue-500 transition">Services</a>
  
		<!-- Discover Us Dropdown -->
		<div class="relative group">
		  <div class="flex items-center cursor-pointer hover:text-blue-500 transition">
			<span>Discover Us</span>
			<svg class="ml-1 w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
			  <path d="M19 9l-7 7-7-7" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
			</svg>
		  </div>
		  <div class="absolute left-0 mt-2 w-56 bg-white/90 dark:bg-gray-900/90 shadow-md rounded-md opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-300 ease-out">
			<a href="about-us" class="block px-4 py-2 hover:bg-gray-400 dark:hover:bg-gray-400">About Us</a>
			<a href="blog" class="block px-4 py-2 hover:bg-gray-400 dark:hover:bg-gray-400">Blog</a>
			<a href="contact-us" class="block px-4 py-2 hover:bg-gray-400 dark:hover:bg-gray-400">Contact Us</a>
			<a href="store-location" class="block px-4 py-2 hover:bg-gray-400 dark:hover:bg-gray-400">Store Location</a>
		  </div>
		</div>
	  </div>
  
	  <!-- Dark Mode Toggle -->
	  <div class="flex items-center space-x-3">
		<label for="menu-toggle" class="lg:hidden cursor-pointer ml-3">
		  <svg class="w-6 h-6 text-gray-900 dark:text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
			<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
		  </svg>
		</label>
	  </div>
	</div>
  </nav>
  
  <!-- Toggle Checkbox -->
  <input type="checkbox" id="menu-toggle" class="peer hidden" autocomplete="off" />
  
  <!-- Hamburger Icon -->
  <label for="menu-toggle" class="z-50 bg-white/80 backdrop-blur-lg p-3 rounded-full cursor-pointer lg:hidden hover:bg-white/90 transition">
	<svg class="w-6 h-6 text-gray-800" fill="none" viewBox="0 0 24 24" stroke="currentColor">
	  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
	</svg>
  </label>
  
  <!-- Mobile Menu Panel -->
  <div class="fixed top-4 left-1/2 -translate-x-1/2 z-50 w-[90%] max-w-xs bg-white/80 dark:bg-gray-900/90 backdrop-blur-lg shadow-lg rounded-xl px-4 py-4 opacity-0 scale-95 -translate-y-4 peer-checked:opacity-100 peer-checked:scale-100 peer-checked:translate-y-0 transition-all duration-300 ease-out hidden peer-checked:flex flex-col space-y-3 lg:hidden">
	<!-- Header -->
	<div class="flex items-center justify-between">
	  <a href="./">
		<img src="assets/image/logo glint.png" alt="Logo" class="h-12 w-auto" />
	  </a>
	  <label for="menu-toggle" class="p-2 rounded-md text-gray-700 cursor-pointer">
		<svg class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
		  <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
		</svg>
	  </label>
	</div>
  
	<!-- Navigation -->
	<nav class="flex flex-col items-start space-y-2 pt-2 text-lg">
	  <a href="./" class="block w-full rounded-md px-4 py-2 font-medium text-gray-900 dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 transition">Home</a>
  
	  <!-- Products Dropdown -->
	  <div class="w-full">
		<input type="checkbox" id="dropdown-products" class="peer hidden" />
		<label for="dropdown-products" class="flex items-center justify-between w-full px-4 py-2 font-medium text-gray-900 dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 cursor-pointer transition">
		  <a href="product" class="w-full">
			<span>Products</span>
		  </a>
		  <svg class="h-4 w-4 text-gray-800 dark:text-white transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
			<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
		  </svg>
		</label>
		<div class="overflow-hidden max-h-0 peer-checked:max-h-40 transition-all duration-300 ease-in-out">
		  <ul class="py-1 text-lg font-semibold text-gray-700 dark:text-white">
			<li><a href="tshirt" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-700">T-Shirt</a></li>
			<li><a href="jacket" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-700">Jacket</a></li>
			<li><a href="shirts" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-700">Shirt</a></li>
		  </ul>
		</div>
	  </div>
  
	  <a href="services" class="block w-full rounded-md px-4 py-2 font-medium text-gray-900 dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 transition">Services</a>
  
	  <!-- Discover Us Dropdown -->
	  <div class="w-full">
		<input type="checkbox" id="dropdown-discover" class="peer hidden" />
		<label for="dropdown-discover" class="flex items-center justify-between w-full px-4 py-2 font-medium text-gray-900 dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 cursor-pointer transition">
		  <span>Discover Us</span>
		  <svg class="h-4 w-4 text-gray-800 dark:text-white transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
			<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
		  </svg>
		</label>
		<div class="overflow-hidden max-h-0 peer-checked:max-h-60 transition-all duration-300 ease-in-out">
		  <ul class="py-1 text-lg font-semibold text-gray-700 dark:text-white">
			<li><a href="about-us" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-700">About Us</a></li>
			<li><a href="blog" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-700">Blog</a></li>
			<li><a href="contact-us" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-700">Contact Us</a></li>
			<li><a href="store-location" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-700">Store Location</a></li>
		  </ul>
		</div>
	  </div>
	</nav>
  </div>
  