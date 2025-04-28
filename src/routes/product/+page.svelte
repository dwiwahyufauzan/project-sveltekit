<script>
    import '../../app.css';
  </script>
  
    <style type="text/tailwindcss"></style>
    <div class="bg-gray-900">
  <header class="fixed top-4 left-1/2 transform -translate-x-1/2 z-50 w-full max-w-screen-lg bg-white shadow-sm border border-gray-300 rounded-full px-4">
    <nav class="flex items-center justify-between px-4 py-2">
      
      <!-- Logo -->
      <a href="/" class="flex items-center -m-1.5 p-1.5">
        <span class="sr-only">Your Company</span>
        <img src="assets/image/logo glint.png" alt="Your Company Logo" class="h-14 w-14 object-contain">
      </a>

      <!-- Desktop Menu -->
      <div class="hidden lg:flex lg:gap-x-8">
        <a href="/" class="text-lg font-semibold text-gray-900">Home</a>

        <!-- Products Dropdown -->
        <div class="relative group">
          <a href="/product" class="inline-flex items-center text-lg font-semibold text-blue-400 px-3 group-hover:text-blue-500 transition cursor-pointer">
            <span>Products</span>
            <svg class="ml-2 h-5 w-5 text-blue-400 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
            </svg>
          </a>
          <div class="absolute left-0 mt-2 w-52 bg-white shadow-lg rounded-lg z-50 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-200 ease-in-out">
            <ul class="py-2 text-lg text-gray-700">
              <li><a href="/tshirts" class="block px-6 py-3 hover:bg-gray-100">T-shirt</a></li>
              <li><a href="/jacket" class="block px-6 py-3 hover:bg-gray-100">Jacket</a></li>
              <li><a href="/kemeja" class="block px-6 py-3 hover:bg-gray-100">Shirt</a></li>
            </ul>
          </div>
        </div>

        <a href="/features" class="text-lg font-semibold text-gray-900">Services</a>

        <!-- Discover Us Dropdown -->
        <div class="relative group">
          <a href="#" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 group-hover:text-blue-500 transition cursor-pointer">
            <span>Discover Us</span>
            <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
            </svg>
          </a>
          <div class="absolute left-0 mt-2 w-52 bg-white shadow-lg rounded-lg z-50 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-200 ease-in-out">
            <ul class="py-2 text-lg text-gray-700">
              <li><a href="/company" class="block px-6 py-3 hover:bg-gray-100">About Us</a></li>
              <li><a href="/blog" class="block px-6 py-3 hover:bg-gray-100">Blog</a></li>
              <li><a href="/contact-us" class="block px-6 py-3 hover:bg-gray-100">Contact Us</a></li>
              <li><a href="/lokasi" class="block px-6 py-3 hover:bg-gray-100">Store Location</a></li>
            </ul>
          </div>
        </div>
      </div>

      <!-- Mobile Menu Toggle -->
      <input type="checkbox" id="menu-toggle" class="peer hidden" />
      <label for="menu-toggle" class="z-50 bg-white/80 backdrop-blur-lg p-4 rounded-full cursor-pointer lg:hidden hover:bg-white/90 transition">
        <svg class="w-7 h-7 text-gray-800" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </label>

      <!-- Mobile Menu Overlay -->
      <div class="fixed inset-0 z-40 bg-black/40 hidden peer-checked:block lg:hidden"></div>

      <!-- Mobile Menu Panel -->
      <div class="fixed top-0 left-0 right-0 z-50 w-full bg-white/90 backdrop-blur-lg shadow-lg rounded-b-2xl px-6 py-5 transform -translate-y-full peer-checked:translate-y-0 transition-transform duration-300 ease-in-out hidden peer-checked:flex flex-col space-y-4 lg:hidden">
        
        <!-- Top Section -->
        <div class="flex items-center justify-between">
          <a href="/">
            <img src="assets/image/logo glint.png" alt="Logo" class="h-10 w-auto">
          </a>
          <label for="menu-toggle" class="p-2 rounded-md text-gray-700 cursor-pointer">
            <svg class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
            </svg>
          </label>
        </div>

        <!-- Menu Items -->
        <nav class="flex flex-col items-start space-y-1 pt-2 text-lg">
          <a href="/" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50">Home</a>

          <!-- Mobile Products Dropdown -->
          <div class="relative w-full">
            <input type="checkbox" id="dropdown-toggle" class="peer hidden" />
            <div class="flex items-center -mx-2 px-3 py-1.5 rounded-md font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
              <a href="/product" class="flex-grow">Products</a>
              <label for="dropdown-toggle">
                <svg class="h-4 w-4 text-gray-800 peer-checked:rotate-180 transition-transform" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                </svg>
              </label>
            </div>
            <div class="absolute left-0 mt-1 w-48 bg-white shadow-md rounded-md z-50 opacity-0 invisible peer-checked:opacity-100 peer-checked:visible transition-all duration-200 ease-in-out">
              <ul class="py-1 text-sm text-gray-700">
                <li><a href="/tshirts" class="block px-4 py-1.5 hover:bg-gray-100">T-Shirt</a></li>
                <li><a href="/jacket" class="block px-4 py-1.5 hover:bg-gray-100">Jacket</a></li>
                <li><a href="/kemeja" class="block px-4 py-1.5 hover:bg-gray-100">Shirt</a></li>
              </ul>
            </div>
          </div>

          <a href="/features" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50">Services</a>

          <!-- Mobile Discover Us Dropdown -->
          <div class="relative w-full">
            <input type="checkbox" id="dropdown" class="peer hidden" />
            <div class="flex items-center -mx-2 px-3 py-1.5 rounded-md font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
              <a href="#" class="flex-grow">Discover Us</a>
              <label for="dropdown">
                <svg class="h-4 w-4 text-gray-800 peer-checked:rotate-180 transition-transform" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                </svg>
              </label>
            </div>
            <div class="absolute left-0 mt-1 w-48 bg-white shadow-md rounded-md z-50 opacity-0 invisible peer-checked:opacity-100 peer-checked:visible transition-all duration-200 ease-in-out">
              <ul class="py-1 text-sm text-gray-700">
                <li><a href="/company" class="block px-4 py-1.5 hover:bg-gray-100">About Us</a></li>
                <li><a href="/blog" class="block px-4 py-1.5 hover:bg-gray-100">Blog</a></li>
                <li><a href="/contact-us" class="block px-4 py-1.5 hover:bg-gray-100">Contact Us</a></li>
                <li><a href="/lokasi" class="block px-4 py-1.5 hover:bg-gray-100">Store Location</a></li>
              </ul>
            </div>
          </div>
        </nav>
      </div>
    </nav>
  </header>

  <!-- Hero Section -->
  <div class="relative isolate overflow-hidden pt-6">
    <img src="https://img.freepik.com/free-photo/family-tailors-having-leather-industry_1303-23397.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740"
         alt="" class="absolute inset-0 -z-10 w-full h-full object-cover">
    <div class="absolute inset-0 -z-10 bg-black/50"></div>

    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-24 text-center">
        <div class="hidden sm:mb-8 sm:flex sm:justify-center">
          <div class="relative rounded-full px-3 py-1 text-sm text-gray-400 ring-1 ring-white/10 hover:ring-white/20">
            Jelajahi beragam produk dari Konveksi Glam Stitch.
            <a href="/product" class="font-semibold text-white">
              <span class="absolute inset-0" aria-hidden="true"></span>Lihat Produk <span aria-hidden="true">&rarr;</span>
            </a>
          </div>
        </div>
        <h1 class="text-5xl sm:text-7xl font-semibold tracking-tight text-white">
          Produk Berkualitas dari Glam Stitch
        </h1>
        <p class="mt-8 text-lg sm:text-xl font-medium text-gray-400">
          Temukan kaos polos, jaket, dan kemeja dengan desain menarik, bahan terbaik, dan jahitan rapi — cocok untuk brand, komunitas, maupun usaha Anda.
        </p>
        <div class="mt-10 flex justify-center gap-x-6">
          <a href="/product" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-xs hover:bg-indigo-400 focus:outline-indigo-400">Lihat Semua Produk</a>
          <a href="/features" class="text-sm font-semibold text-white">Layanan Kami <span aria-hidden="true">→</span></a>
        </div>
      </div>
    </div>
  </div>
</div>
<!--end header-->

<!--hero section with image on the left-->
<div class="relative bg-white py-12 sm:py-20">
  <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
    <div class="flex flex-col lg:flex-row items-center gap-10">
      
      <!-- Left: Image -->
      <div class="w-full lg:w-1/2">
        <img src="https://img.freepik.com/free-photo/carpenter-works-with-tree_1157-18667.jpg?t=st=1745396381~exp=1745399981~hmac=3613685cfe8fe3d6e558d59ce7476f7b8ef5a2ee5083c5db8c37959e91ce3375&w=1380" alt="Produk Konveksi" class="rounded-lg shadow-lg w-full h-auto object-cover">
      </div>

      <!-- Right: Text Content -->
      <div class="w-full lg:w-1/2 text-center lg:text-left">
        <h2 class="text-4xl sm:text-5xl font-bold text-gray-900 leading-tight">
          Selamat Datang di Konveksi <span class="text-indigo-600">Glam Stitch</span>
        </h2>
        <p class="mt-5 text-lg sm:text-xl leading-relaxed text-gray-700">
          Kami memproduksi kaos polos, jaket custom, dan kemeja berkualitas tinggi untuk brand, komunitas, maupun kebutuhan usaha Anda. Desain stylish, jahitan rapi, hasil maksimal.
        </p>
        <div class="mt-10 flex flex-col sm:flex-row lg:justify-start justify-center gap-4">
          <a href="/features" class="inline-block rounded-md bg-indigo-600 px-6 py-3 text-base font-semibold text-white shadow-md hover:bg-indigo-500 transition">
            Layanan Kami
          </a>
          <a href="/company" class="inline-block rounded-md border border-gray-300 px-6 py-3 text-base font-semibold text-gray-700 hover:bg-gray-100 transition">
            Tentang Kami
          </a>
        </div>
      </div>

    </div>
  </div>
</div>
<!--end hero section-->


<!-- Product Section -->
<div class="bg-white py-20">
  <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-16">
    <div class="text-center mb-14">
      <p class="text-3xl font-extrabold tracking-tight text-gray-900">Koleksi Andalan Kami</p>
      <p class="mt-4 text-lg text-gray-600">Temukan pilihan fashion terbaik dari kami, dibuat dengan kualitas tinggi dan sentuhan desain yang stylish.</p>
    </div>

    <div class="grid grid-cols-1 gap-y-12 gap-x-8 sm:grid-cols-2 lg:grid-cols-3">
      <!-- Kaos Polos -->
      <div class="flex flex-col items-center text-center space-y-6">
        <a href="/tshirts" class="block w-full max-w-sm mx-auto">
          <div class="overflow-hidden rounded-xl shadow-md transition-all duration-300 ease-in-out transform hover:scale-105">
            <img 
              src="https://media.istockphoto.com/id/185941321/id/foto/tubuh-bagian-atas-pria.jpg?s=612x612&w=0&k=20&c=iS9nQtGYKbNusFB7N6ygJZPdkmSvK1OwkhinmalwW3o=" 
              alt="Kaos Polos Glam Stitch" 
              class="w-full aspect-[4/5] object-cover"
            >
          </div>
        </a>        
        <h3 class="text-xl font-semibold text-gray-900">Kaos Polos</h3>
        <p class="text-base text-gray-600 px-4 max-w-sm">Nyaman dipakai seharian, hadir dalam berbagai warna dan bahan premium yang adem dan awet.</p>
      </div>

      <!-- Jaket -->
      <div class="flex flex-col items-center text-center space-y-6">
        <a href="/jacket" class="block w-full max-w-sm mx-auto">
          <div class="overflow-hidden rounded-xl shadow-md transition-all duration-300 ease-in-out transform hover:scale-105">
            <img 
              src="https://media.istockphoto.com/id/2085676478/id/foto/mockup-hoodie-putih-pada-pria-berjanggut-kaus-oversized-dengan-saku-untuk-desain-branding.jpg?s=612x612&w=0&k=20&c=7QKD-7q--IDD5CV0p5JDNuWy6f26zHLa0qCI3cF8wOc=" 
              alt="Jaket Glam Stitch" 
              class="w-full aspect-[4/5] object-cover"
            >
          </div>
        </a>        
        <h3 class="text-xl font-semibold text-gray-900">Jaket</h3>
        <p class="text-base text-gray-600 px-4 max-w-sm">Hangat dan stylish, cocok untuk aktivitas luar ruangan maupun casual harian.</p>
      </div>

      <!-- Kemeja -->
      <div class="flex flex-col items-center text-center space-y-6">
        <a href="/kemeja" class="block w-full max-w-sm mx-auto">
          <div class="overflow-hidden rounded-xl shadow-md transition-all duration-300 ease-in-out transform hover:scale-105">
            <img 
              src="https://img.freepik.com/free-photo/business-casual-shirt-white-closeup-outdoor-photoshoot_53876-119744.jpg?ga=GA1.1.1868222757.1738365469&w=740" 
              alt="Kemeja Glam Stitch" 
              class="w-full aspect-[4/5] object-cover"
            >
          </div>
        </a>        
        <h3 class="text-xl font-semibold text-gray-900">Kemeja</h3>
        <p class="text-base text-gray-600 px-4 max-w-sm">Tampil rapi dan profesional dengan kemeja berkualitas tinggi dari Glam Stitch.</p>
      </div>
    </div>
  </div>
</div>



<!--end product sections-->

<!-- ,reviews sections-->
<section class="bg-gradient-to-b from-white via-gray-50 to-white py-24">
  <div class="max-w-7xl mx-auto px-6 lg:px-16">
    <div class="text-center">
      <h2 class="text-4xl sm:text-2xl font-extrabold text-gray-900">Apa Kata Mereka?</h2>
      <p class="mt-4 text-lg text-gray-600">Review dari para pelanggan setia kami.</p>
    </div>

    <div class="mt-16 grid gap-10 sm:grid-cols-2 lg:grid-cols-3">
      
      <!-- Review Card -->
      <div class="bg-white shadow-xl rounded-3xl p-8 border border-gray-100 hover:shadow-2xl transition-all duration-300">
        <div class="flex items-center gap-4 mb-4">
          <img class="w-12 h-12 rounded-full object-cover border-2 border-indigo-500" src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Putri Aulia">
          <div>
            <h4 class="font-semibold text-gray-900 text-base">Putri Aulia</h4>
            <span class="text-sm text-indigo-600 font-medium bg-indigo-50 rounded-full px-2 py-0.5">Kaos Polos</span>
          </div>
        </div>

        <div class="flex items-center mb-3">
          <!-- Stars -->
          <div class="flex space-x-1 text-yellow-400">
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5 text-gray-300" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
          </div>
        </div>

        <p class="text-gray-700 leading-relaxed text-sm">“Kaos polosnya super nyaman dipakai seharian. Bahannya adem, jahitannya rapi, dan warnanya nggak gampang pudar!”</p>
      </div>
      <div class="bg-white shadow-xl rounded-3xl p-8 border border-gray-100 hover:shadow-2xl transition-all duration-300">
        <div class="flex items-center gap-4 mb-4">
          <img class="w-12 h-12 rounded-full object-cover border-2 border-indigo-500" src="https://media.istockphoto.com/id/483627817/id/foto/memamerkan-putih-mutiaranya.jpg?s=612x612&w=0&k=20&c=0dXbdlR-Ten2QPyJ7E6WtpRjGAwLFLbfWywDJ0RCs_E=" alt="Putri Aulia">
          <div>
            <h4 class="font-semibold text-gray-900 text-base">Arifki Pratama</h4>
            <span class="text-sm text-indigo-600 font-medium bg-indigo-50 rounded-full px-2 py-0.5">Jaket</span>
          </div>
        </div>
      
        <div class="flex items-center mb-3">
          <!-- Stars -->
          <div class="flex space-x-1 text-yellow-400">
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
          </div>
        </div>
      
        <p class="text-gray-700 leading-relaxed text-sm">“Jaket dari Glam Stitch bener-bener keren! Bahannya tebal tapi tetap ringan, potongannya pas, dan sangat cocok buat gaya harian yang casual tapi tetap kece.”</p>
      </div>
      <div class="bg-white shadow-xl rounded-3xl p-8 border border-gray-100 hover:shadow-2xl transition-all duration-300">
        <div class="flex items-center gap-4 mb-4">
          <img class="w-12 h-12 rounded-full object-cover border-2 border-indigo-500" src="https://media.istockphoto.com/id/1325882419/id/foto/wanita-meniup-ciuman-udara-pada-latar-belakang-biru-muda.jpg?s=612x612&w=0&k=20&c=xBVLOjJkZ2AAPBMi-bPeYzDKTQLQq48z0xPpWb7rUVE=" alt="Putri Aulia">
          <div>
            <h4 class="font-semibold text-gray-900 text-base">Firda Aulia</h4>
            <span class="text-sm text-indigo-600 font-medium bg-indigo-50 rounded-full px-2 py-0.5">Jaket</span>
          </div>
        </div>
      
        <div class="flex items-center mb-3">
          <!-- Stars -->
          <div class="flex space-x-1 text-yellow-400">
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09L5.5 12.18.5 7.91l6.064-.88L10 2l3.436 5.03L19.5 7.91l-5 4.27 1.378 5.91z"/></svg>
          </div>
        </div>
      
        <p class="text-gray-700 leading-relaxed text-sm">“Kemejanya elegan banget! Bahannya adem, jatuhnya bagus di badan, dan jahitannya rapi. Cocok banget buat acara formal maupun nongkrong santai.”</p>

      </div>
      

      <!-- Tambah review lainnya di sini dengan struktur yang sama -->
      <!-- Gunakan nama, foto, produk, dan teks ulasan yang berbeda agar beragam -->

    </div>
  </div>
</section>

<!--end reviews sections-->

<!--logo clouds-->
<div class="bg-gray-900 py-24 sm:py-24 rounded-t-4xl">
  <div class="mx-auto max-w-7xl px-6 lg:px-8">
    <div class="mx-auto grid max-w-lg grid-cols-4 items-center gap-x-8 gap-y-12 sm:max-w-xl sm:grid-cols-6 sm:gap-x-10 sm:gap-y-14 lg:mx-0 lg:max-w-none lg:grid-cols-5">
      <img class="col-span-2 max-h-12 w-full object-contain lg:col-span-1" src="https://tailwindcss.com/plus-assets/img/logos/158x48/transistor-logo-white.svg" alt="Transistor" width="158" height="48">
      <img class="col-span-2 max-h-12 w-full object-contain lg:col-span-1" src="https://tailwindcss.com/plus-assets/img/logos/158x48/reform-logo-white.svg" alt="Reform" width="158" height="48">
      <img class="col-span-2 max-h-12 w-full object-contain lg:col-span-1" src="https://tailwindcss.com/plus-assets/img/logos/158x48/tuple-logo-white.svg" alt="Tuple" width="158" height="48">
      <img class="col-span-2 max-h-12 w-full object-contain sm:col-start-2 lg:col-span-1" src="https://tailwindcss.com/plus-assets/img/logos/158x48/savvycal-logo-white.svg" alt="SavvyCal" width="158" height="48">
      <img class="col-span-2 col-start-2 max-h-12 w-full object-contain sm:col-start-auto lg:col-span-1" src="https://tailwindcss.com/plus-assets/img/logos/158x48/statamic-logo-white.svg" alt="Statamic" width="158" height="48">
    </div>
    <div class="mt-16 flex justify-center">
      <p class="relative rounded-full bg-gray-800 px-4 py-1.5 text-sm/6 text-gray-300">
        <span class="hidden md:inline">Konveksi Glam Stitch dipercaya oleh banyak brand ternama.</span>
        <a href="#" class="font-semibold text-white"><span class="absolute inset-0" aria-hidden="true"></span> Lihat cerita pelanggan kami <span aria-hidden="true">&rarr;</span></a>
      </p>
    </div>
  </div>
</div>
<!--end logo clouds sections-->

<!--footers-->
<footer class="bg-gray-900" aria-labelledby="footer-heading">
  <h2 id="footer-heading" class="sr-only">Footer</h2>
  <div class="mx-auto max-w-7xl px-6 pb-8 pt-16 sm:pt-24 lg:px-8">
    <div class="xl:grid xl:grid-cols-3 xl:gap-8">
      <!-- Logo & Description -->
      <div class="space-y-8">
        <img class="h-20 w-20" src="assets/image/logo glint.png" alt="Glam Stitch Logo">
        <p class="text-sm leading-6 text-gray-300">
          Glam Stitch adalah mitra konveksi terpercaya untuk kebutuhan baju custom, seragam, dan merchandise Anda. Kualitas terbaik, harga bersaing.
        </p>
        <div class="flex space-x-6">
          <a href="#" class="text-gray-500 hover:text-gray-400">
            <span class="sr-only">Facebook</span>
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
              <path d="M22 12a10 10 0 10-11.6 9.87v-6.99H8.1v-2.88h2.3V9.41c0-2.28 1.35-3.55 3.42-3.55.99 0 2.03.18 2.03.18v2.24h-1.14c-1.12 0-1.47.7-1.47 1.42v1.71h2.5l-.4 2.88h-2.1v6.99A10 10 0 0022 12z"/>
            </svg>
          </a>
          <a href="#" class="text-gray-500 hover:text-gray-400">
            <span class="sr-only">Instagram</span>
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
              <path d="M7 2C4.24 2 2 4.24 2 7v10c0 2.76 2.24 5 5 5h10c2.76 0 5-2.24 5-5V7c0-2.76-2.24-5-5-5H7zm10 2c1.66 0 3 1.34 3 3v10c0 1.66-1.34 3-3 3H7c-1.66 0-3-1.34-3-3V7c0-1.66 1.34-3 3-3h10zm-5 3a5 5 0 100 10 5 5 0 000-10zm0 2a3 3 0 110 6 3 3 0 010-6zm4.5-1a1 1 0 100 2 1 1 0 000-2z"/>
            </svg>
          </a>
        </div>
      </div>

      <!-- Link Sections -->
      <div class="mt-16 grid grid-cols-2 gap-8 sm:grid-cols-3 xl:col-span-2 xl:mt-0">
        <div>
          <h3 class="text-sm font-semibold leading-6 text-white">Produk & Layanan</h3>
          <ul role="list" class="mt-6 space-y-4">
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Katalog Produk</a></li>
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Jasa Sablon & Bordir</a></li>
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Custom Desain Baju</a></li>
          </ul>
        </div>
        <div>
          <h3 class="text-sm font-semibold leading-6 text-white">Bantuan</h3>
          <ul role="list" class="mt-6 space-y-4">
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Cara Pemesanan</a></li>
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">FAQ</a></li>
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Hubungi Kami</a></li>
          </ul>
        </div>
        <div>
          <h3 class="text-sm font-semibold leading-6 text-white">Tentang Kami</h3>
          <ul role="list" class="mt-6 space-y-4">
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Profil Perusahaan</a></li>
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Testimoni Pelanggan</a></li>
            <li><a href="#" class="text-sm leading-6 text-gray-300 hover:text-white">Karir</a></li>
          </ul>
        </div>
      </div>
    </div>

    <!-- Copyright -->
    <div class="mt-16 border-t border-white/10 pt-8 sm:mt-20 lg:mt-24">
      <p class="text-xs leading-5 text-gray-400">&copy; 2025 Glam Stitch. All rights reserved.</p>
    </div>
  </div>
</footer>