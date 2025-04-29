<script>
    import '../app.css';
  </script>
  
    <style type="text/tailwindcss"></style>
    <!-- Header -->
<div class="bg-gray-900">
    <header class="fixed top-4 left-1/2 transform -translate-x-1/2 z-50 w-full max-w-screen-lg bg-white shadow-sm border border-gray-300 rounded-full px-4">
      <nav class="flex items-center justify-between px-4 py-2">
        
        <!-- Logo -->
        <a href="/project-sveltekit/" class="flex items-center -m-1.5 p-1.5">
          <span class="sr-only">Your Company</span>
          <img class="h-14 w-14 object-contain" src="assets/image/logo glint.png" alt="Your Company Logo">
        </a>
  
        <!-- Desktop Menu -->
        <div class="hidden lg:flex lg:gap-x-8">
          <a href="/project-sveltekit/" class="text-lg font-semibold text-blue-400">Home</a>
  
          <!-- Products Dropdown (Desktop) -->
          <div class="relative group">
            <a href="/project-sveltekit/product" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 group-hover:text-blue-500 transition">
              <span>Products</span>
              <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none"
                viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
              </svg>
            </a>
            <div class="absolute left-0 mt-2 w-52 bg-white shadow-lg rounded-lg z-50 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-200 ease-in-out">
              <ul class="py-2 text-lg text-gray-700">
                <li><a href="/project-sveltekit/tshirts" class="block px-6 py-3 hover:bg-gray-100">T-shirt</a></li>
                <li><a href="/project-sveltekit/jacket" class="block px-6 py-3 hover:bg-gray-100">Jacket</a></li>
                <li><a href="/project-sveltekit/kemeja" class="block px-6 py-3 hover:bg-gray-100">Shirt</a></li>
              </ul>
            </div>
          </div>
  
          <a href="/project-sveltekit/features" class="text-lg font-semibold text-gray-900">Services</a>
  
          <!-- Discover Us Dropdown -->
          <div class="relative group">
            <a href="/project-sveltekit#" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 group-hover:text-blue-500 transition">
              <span>Discover Us</span>
              <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none"
                viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
              </svg>
            </a>
            <div class="absolute left-0 mt-2 w-52 bg-white shadow-lg rounded-lg z-50 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-200 ease-in-out">
              <ul class="py-2 text-lg text-gray-700">
                <li><a href="/project-sveltekit/company" class="block px-6 py-3 hover:bg-gray-100">About Us</a></li>
              <li><a href="/project-sveltekit/blog" class="block px-6 py-3 hover:bg-gray-100">Blog</a></li>
              <li><a href="/project-sveltekit/contact-us" class="block px-6 py-3 hover:bg-gray-100">Contact Us</a></li>
              <li><a href="/project-sveltekit/lokasi" class="block px-6 py-3 hover:bg-gray-100">Store Location</a></li>
            </ul>
            </div>
          </div>
        </div>
  
        <!-- Mobile Menu Toggle -->
        <input type="checkbox" id="menu-toggle" class="peer hidden" autocomplete="off" />
        <label for="menu-toggle" class="z-50 bg-white/80 backdrop-blur-lg p-4 rounded-full cursor-pointer lg:hidden hover:bg-white/90 transition">
          <svg class="w-7 h-7 text-gray-800" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </label>
  
        <!-- Mobile Menu Panel -->
        <div class="fixed top-0 left-0 right-0 z-50 w-full bg-white/90 backdrop-blur-lg shadow-lg rounded-b-2xl px-6 py-5 transform -translate-y-full peer-checked:translate-y-0 transition-transform duration-300 ease-in-out hidden peer-checked:flex flex-col space-y-4 lg:hidden">
          <div class="flex items-center justify-between">
            <a href="/project-sveltekit/">
              <img src="assets/image/logo glint.png" alt="Logo" class="h-10 w-auto">
            </a>
            <label for="menu-toggle" class="p-2 rounded-md text-gray-700 cursor-pointer">
              <svg class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
              </svg>
            </label>
          </div>
  
          <!-- Mobile Nav -->
          <nav class="flex flex-col items-start space-y-1 pt-2 text-lg">
            <a href="/project-sveltekit/" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 transition">Home</a>
  
            <!-- Mobile Products Dropdown -->
            <div class="relative w-full">
              <input type="checkbox" id="dropdown-toggle" class="peer hidden" />
              <div class="flex items-center -mx-2 rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
                <a href="/project-sveltekit/product" class="flex-grow">Products</a>
                <label for="dropdown-toggle">
                  <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none"
                    viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                  </svg>
                </label>
              </div>
              <div class="absolute left-0 mt-1 w-48 bg-white shadow-md rounded-md z-50 opacity-0 invisible peer-checked:opacity-100 peer-checked:visible transition-all duration-200 ease-in-out">
                <ul class="py-1 text-sm text-gray-700">
                    <li><a href="/project-sveltekit/tshirts" class="block px-4 py-1.5 hover:bg-gray-100">T-Shirt</a></li>
                    <li><a href="/project-sveltekit/jacket" class="block px-4 py-1.5 hover:bg-gray-100">Jacket</a></li>
                    <li><a href="/project-sveltekit/kemeja" class="block px-4 py-1.5 hover:bg-gray-100">Shirt</a></li>
                  </ul>
              </div>
            </div>
  
            <a href="/project-sveltekit/features" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 transition">Services</a>
  
            <!-- Mobile Discover Us Dropdown -->
            <div class="relative w-full">
              <input type="checkbox" id="dropdown" class="peer hidden" />
              <div class="flex items-center -mx-2 rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
                <a href="/project-sveltekit#" class="flex-grow">Discover Us</a>
                <label for="dropdown">
                  <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none"
                    viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                  </svg>
                </label>
              </div>
              <div class="absolute left-0 mt-1 w-48 bg-white shadow-md rounded-md z-50 opacity-0 invisible peer-checked:opacity-100 peer-checked:visible transition-all duration-200 ease-in-out">
                <ul class="py-1 text-sm text-gray-700">
                  <li><a href="/project-sveltekit/company" class="block px-4 py-1.5 hover:bg-gray-100">About Us</a></li>
                  <li><a href="/project-sveltekit/blog" class="block px-4 py-1.5 hover:bg-gray-100">Blog</a></li>
                  <li><a href="/project-sveltekit/contact-us" class="block px-4 py-1.5 hover:bg-gray-100">Contact Us</a></li>
                  <li><a href="/project-sveltekit/lokasi" class="block px-4 py-1.5 hover:bg-gray-100">Store Location</a></li>
                </ul>
              </div>
            </div>
          </nav>
        </div>
      </nav>
    </header>
  
    <!-- Hero Section -->
    <div class="relative isolate overflow-hidden pt-6">
      <img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2830&q=80&blend=111827&sat=-100&exp=15&blend-mode=multiply"
        alt="" class="absolute inset-0 -z-10 size-full object-cover">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-24">
          <div class="hidden sm:mb-8 sm:flex sm:justify-center">
            <div class="relative rounded-full px-3 py-1 text-sm/6 text-gray-400 ring-1 ring-white/10 hover:ring-white/20">
              Konveksi Glam Stitch — Produksi pakaian berkualitas tinggi untuk merek Anda.
              <a href="/project-sveltekit/product" class="font-semibold text-white">
                <span class="absolute inset-0" aria-hidden="true"></span>Selengkapnya <span aria-hidden="true">&rarr;</span>
              </a>
            </div>
          </div>
          <div class="text-center">
            <h1 class="text-5xl font-semibold tracking-tight text-white sm:text-7xl">
              Glam Stitch Mitra Konveksi Terpercaya Anda
            </h1>
            <p class="mt-8 text-lg font-medium text-gray-400 sm:text-xl">
              Kami menyediakan layanan produksi pakaian yang terpercaya dan profesional untuk membantu pertumbuhan bisnis Anda — dengan kualitas tinggi, proses cepat, dan harga bersaing.
            </p>
            <div class="mt-10 flex items-center justify-center gap-x-6">
              <a href="/project-sveltekit#" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-xs hover:bg-indigo-400 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-400">Mulai Sekarang</a>
              <a href="/project-sveltekit#" class="text-sm font-semibold text-white">Jelajahi Lebih Lanjut <span aria-hidden="true">→</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- End Header -->
  
  <!--why choose us-->
  <div class="relative isolate overflow-hidden bg-gray-100">
    <div class="absolute top-10 left-[calc(50%-4rem)] -z-10 transform-gpu blur-3xl sm:left-[calc(50%-18rem)] lg:top-[calc(50%-30rem)] lg:left-48 xl:left-[calc(50%-24rem)]" aria-hidden="true">
      <div class="aspect-1108/632 w-[69.25rem] bg-gradient-to-r from-[#80caff] to-[#4f46e5] opacity-20" style="clip-path: polygon(73.6% 51.7%, 91.7% 11.8%, 100% 46.4%, 97.4% 82.2%, 92.5% 84.9%, 75.7% 64%, 55.3% 47.5%, 46.5% 49.4%, 45% 62.9%, 50.3% 87.2%, 21.3% 64.1%, 0.1% 100%, 5.4% 51.1%, 21.4% 63.9%, 58.9% 0.2%, 73.6% 51.7%)"></div>
    </div>
    <div class="mx-auto max-w-7xl px-6 pt-10 pb-24 sm:pb-32 lg:flex lg:items-center lg:justify-between lg:px-16 lg:py-24">
      <!-- Left: Text content -->
      <div class="max-w-2xl">
        <span class="rounded-full bg-indigo-500/10 px-3 py-1 text-sm font-semibold text-indigo-400 ring-1 ring-indigo-500/20 ring-inset">Kenapa Memilih Kami?</span>
        <h1 class="mt-10 text-5xl font-semibold tracking-tight text-pretty text-gray-900 sm:text-6xl">Kenapa Harus Glam Stitch?</h1>
        <p class="mt-6 text-lg font-medium text-pretty text-gray-600 sm:text-xl">
          Kami menghadirkan layanan konveksi berkualitas tinggi dengan proses mudah, hasil presisi, dan pelayanan profesional.
          Glam Stitch adalah solusi terpercaya untuk kebutuhan pakaian custom Anda.
        </p>
        <ul class="mt-6 space-y-3 text-gray-700 text-base leading-relaxed">
          <li>✅ Bahan Berkualitas Premium</li>
          <li>✅ Tim Desain dan Produksi Profesional</li>
          <li>✅ Waktu Pengerjaan Cepat dan Tepat Waktu</li>
          <li>✅ Harga Kompetitif dan Transparan</li>
          <li>✅ Dukungan Konsultasi dan Revisi Desain</li>
        </ul>
        <div class="mt-10 flex items-center gap-x-6">
          <a href="/project-sveltekit/contact-us" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-400 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-400">Hubungi Kami</a>
          <a href="/project-sveltekit/blog" class="text-sm font-semibold text-indigo-600 hover:text-indigo-500">Lihat Portofolio <span aria-hidden="true">→</span></a>
        </div>
      </div>
  
      <!-- Right: Image -->
      <div class="mt-16 lg:mt-0 lg:ml-16 max-w-xl w-full">
        <img class="rounded-xl shadow-xl w-full object-cover" src="assets/image/gambar2.png" alt="Tim produksi Glam Stitch sedang menjahit kaos custom" />
      </div>
    </div>
  </div>
  
  <!--end why choose us-->
  
  <!--how to buy-->
  <div class="bg-white">
    <div class="mx-auto max-w-7xl px-4 py-16 sm:px-6 lg:px-16">
      <h2 class="text-5xl font-semibold tracking-tight text-gray-900 text-center">Cara Pemesanan</h2>
      <p class="mt-4 text-base text-gray-500 text-center">Ikuti langkah mudah berikut untuk memesan produk dari Glam Stitch.</p>
      
      <div class="mt-16 flex flex-col lg:flex-row items-center lg:items-start gap-10">
        <!-- Gambar -->
        <div class="w-full lg:w-1/2">
          <img src="assets/image/gambar4.png" alt="Ilustrasi cara pemesanan" class="w-full h-auto object-contain max-w-md mx-auto lg:mx-0">
        </div>
  
        <!-- Langkah-langkah -->
        <div class="w-full lg:w-1/2 space-y-12">
          <div class="group block">
            <h3 class="text-xl font-semibold text-gray-900">1. Konsultasi</h3>
            <p class="mt-2 text-sm text-gray-500">Hubungi tim kami untuk berdiskusi mengenai desain, bahan, dan kebutuhan Anda. Kami siap memberikan saran terbaik untuk memenuhi permintaan Anda.</p>
          </div>
          <div class="group block">
            <h3 class="text-xl font-semibold text-gray-900">2. Produksi</h3>
            <p class="mt-2 text-sm text-gray-500">Setelah desain disetujui, kami akan memulai proses produksi dengan bahan berkualitas tinggi yang sesuai dengan standar kami. Proses ini dijalankan dengan teknologi modern untuk memastikan hasil yang optimal.</p>
          </div>
          <div class="group block">
            <h3 class="text-xl font-semibold text-gray-900">3. Pengiriman</h3>
            <p class="mt-2 text-sm text-gray-500">Produk jadi akan dikirim ke alamat Anda sesuai estimasi waktu yang telah disepakati. Kami memastikan pengiriman tepat waktu dengan layanan kurir yang terpercaya untuk pengalaman yang lebih nyaman.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
  
  <!--end how to buy-->
  
  <!--size chart-->
  <div class="bg-gray-900 py-6 sm:py-16">
    <div class="mx-auto max-w-7xl px-16 lg:px-16">
      <div class="mx-auto max-w-2xl lg:mx-0">
        <h2 class="text-4xl font-semibold tracking-tight text-pretty text-white sm:text-5xl">Pilih Ukuran yang Tepat untuk Anda</h2>
        <p class="mt-6 text-base/7 text-gray-400">Pilih ukuran pakaian yang sesuai dengan panduan ukuran kami untuk kenyamanan maksimal.</p>
      </div>
      <div class="mx-auto mt-16 flex flex-col gap-8 lg:mx-0 lg:mt-20 lg:max-w-none lg:flex-row lg:items-center justify-center">
        <div class="flex flex-col justify-center items-center gap-x-16 gap-y-8 rounded-2xl bg-gray-50 p-8 sm:w-3/4 sm:max-w-md lg:w-72 lg:max-w-none lg:flex-none lg:flex-col">
          <p class="flex-none text-3xl font-bold tracking-tight text-gray-900">T-Shirt</p>
          <div class="sm:w-80 sm:shrink lg:w-auto lg:flex-none text-center">
            <img src="assets/image/gambar5.png" alt="T-Shirt" class="rounded-2xl">
            <p class="text-lg font-semibold tracking-tight text-gray-900">Ukuran T-Shirt</p>
            <p class="mt-2 text-base/7 text-gray-600">Pilih ukuran sesuai dengan ukuran dada dan panjang badan Anda.</p>
          </div>
        </div>
        <div class="flex flex-col justify-center items-center gap-x-16 gap-y-8 rounded-2xl bg-gray-50 p-8 sm:w-3/4 sm:max-w-md lg:w-72 lg:max-w-none lg:flex-none lg:flex-col">
          <p class="flex-none text-3xl font-bold tracking-tight text-gray-900">Jaket</p>
          <div class="sm:w-80 sm:shrink lg:w-auto lg:flex-none text-center">
            <img src="assets/image/gambar6.png" alt="Jacket" class="rounded-2xl">
            <p class="text-lg font-semibold tracking-tight text-gray-900">Ukuran Jaket</p>
            <p class="mt-2 text-base/7 text-gray-600">Pilih ukuran sesuai dengan ukuran dada dan panjang badan Anda.</p>
          </div>
        </div>
        <div class="flex flex-col justify-center items-center gap-x-16 gap-y-8 rounded-2xl bg-gray-50 p-8 sm:w-3/4 sm:max-w-md lg:w-72 lg:max-w-none lg:flex-none lg:flex-col">
          <p class="flex-none text-3xl font-bold tracking-tight text-gray-900">Kemeja</p>
          <div class="sm:w-80 sm:shrink lg:w-auto lg:flex-none text-center">
            <img src="assets/image/gambar7.png" alt="Shirt" class="rounded-2xl">
            <p class="text-lg font-semibold tracking-tight text-gray-900">Ukuran Kemeja</p>
            <p class="mt-2 text-base/7 text-gray-600">Pilih ukuran sesuai dengan ukuran dada dan panjang badan Anda.</p>
          </div>
        </div>
      </div>
    </div>  
  </div>
  <!--end size chart-->
  
  <!--stats-->
  <div class="relative isolate overflow-hidden bg-gray-100">
    <div class="absolute top-10 left-[calc(50%-4rem)] -z-10 transform-gpu blur-3xl sm:left-[calc(50%-18rem)] lg:top-[calc(50%-30rem)] lg:left-48 xl:left-[calc(50%-24rem)]" aria-hidden="true">
      <div class="aspect-1108/632 w-[69.25rem] bg-gradient-to-r from-[#80caff] to-[#4f46e5] opacity-20" style="clip-path: polygon(73.6% 51.7%, 91.7% 11.8%, 100% 46.4%, 97.4% 82.2%, 92.5% 84.9%, 75.7% 64%, 55.3% 47.5%, 46.5% 49.4%, 45% 62.9%, 50.3% 87.2%, 21.3% 64.1%, 0.1% 100%, 5.4% 51.1%, 21.4% 63.9%, 58.9% 0.2%, 73.6% 51.7%)"></div>
    </div>
    <div class="mx-auto max-w-7xl px-6 pt-10 pb-24 sm:pb-32 lg:flex lg:items-center lg:justify-between lg:px-16 lg:py-24">
      <!-- Left: Text content -->
      <div class="max-w-4xl mx-auto px-4 py-10">
        
        <!-- Section Heading -->
        <div class="text-center mb-12">
          <h2 class="text-4xl font-extrabold text-gray-900 sm:text-5xl mb-4">Pencapaian Glam Stitch</h2>
          <p class="text-lg text-gray-600">Dedikasi kami tercermin dari data. Berikut pencapaian kami dalam melayani kebutuhan fashion Anda.</p>
        </div>
  
        <!-- Statistik -->
        <div class="grid grid-cols-1 sm:grid-cols-3 gap-10 text-center py-12 max-w-6xl mx-auto px-4">
          <!-- Pengguna -->
          <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
            <div class="w-20 h-20 flex items-center justify-center bg-yellow-400/20 rounded-full text-yellow-600 text-4xl">
              👤
            </div>
            <div>
              <p class="mt-4 text-4xl font-extrabold text-gray-800">1000+</p>
              <p class="text-lg sm:text-xl text-gray-500">Pengguna</p>
            </div>
          </div>
          
          <!-- Pesanan -->
          <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
            <div class="w-20 h-20 flex items-center justify-center bg-yellow-400/20 rounded-full text-yellow-600 text-4xl">
              📦
            </div>
            <div>
              <p class="mt-4 text-4xl font-extrabold text-gray-800">45000+</p>
              <p class="text-lg sm:text-xl text-gray-500">Pesanan</p>
            </div>
          </div>
  
          <!-- Pengalaman -->
          <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
            <div class="w-20 h-20 flex items-center justify-center bg-yellow-400/20 rounded-full text-yellow-600 text-4xl">
              📅
            </div>
            <div>
              <p class="mt-4 text-4xl font-extrabold text-gray-800">5+ Tahun</p>
              <p class="text-lg sm:text-xl text-gray-500">Pengalaman</p>
            </div>
          </div>
        </div>
  
      </div>    
    </div>
  </div>
  <!--end header-->
  
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
          <a href="/project-sveltekit#" class="font-semibold text-white"><span class="absolute inset-0" aria-hidden="true"></span> Lihat cerita pelanggan kami <span aria-hidden="true">&rarr;</span></a>
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
            <a href="/project-sveltekit#" class="text-gray-500 hover:text-gray-400">
              <span class="sr-only">Facebook</span>
              <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                <path d="M22 12a10 10 0 10-11.6 9.87v-6.99H8.1v-2.88h2.3V9.41c0-2.28 1.35-3.55 3.42-3.55.99 0 2.03.18 2.03.18v2.24h-1.14c-1.12 0-1.47.7-1.47 1.42v1.71h2.5l-.4 2.88h-2.1v6.99A10 10 0 0022 12z"/>
              </svg>
            </a>
            <a href="/project-sveltekit#" class="text-gray-500 hover:text-gray-400">
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
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Katalog Produk</a></li>
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Jasa Sablon & Bordir</a></li>
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Custom Desain Baju</a></li>
            </ul>
          </div>
          <div>
            <h3 class="text-sm font-semibold leading-6 text-white">Bantuan</h3>
            <ul role="list" class="mt-6 space-y-4">
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Cara Pemesanan</a></li>
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">FAQ</a></li>
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Hubungi Kami</a></li>
            </ul>
          </div>
          <div>
            <h3 class="text-sm font-semibold leading-6 text-white">Tentang Kami</h3>
            <ul role="list" class="mt-6 space-y-4">
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Profil Perusahaan</a></li>
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Testimoni Pelanggan</a></li>
              <li><a href="/project-sveltekit#" class="text-sm leading-6 text-gray-300 hover:text-white">Karir</a></li>
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
