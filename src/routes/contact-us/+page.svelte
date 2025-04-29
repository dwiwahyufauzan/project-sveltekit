<script>
    import '../../app.css';
  </script>
  
    <style type="text/tailwindcss"></style>
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
              <a href="/project-sveltekit/" class="text-lg font-semibold text-gray-900">Home</a>
      
              <!-- Products Dropdown -->
              <div class="relative group">
                <a href="/project-sveltekit/product" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 cursor-pointer group-hover:text-blue-500 transition">
                  <span>Products</span>
                  <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
                <a href="/project-sveltekit/#" class="inline-flex items-center text-lg font-semibold text-blue-400 px-3 cursor-pointer group-hover:text-blue-500 transition">
                  <span>Discover Us</span>
                  <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
            <label for="menu-toggle" class="z-50 bg-white/80 backdrop-blur-lg p-4 rounded-full cursor-pointer lg:hidden hover:bg-white/90 transition-all duration-300">
              <svg class="w-7 h-7 text-gray-800" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
              </svg>
            </label>
      
            <!-- Mobile Menu Overlay -->
            <div class="fixed inset-0 z-40 bg-black/40 hidden peer-checked:block lg:hidden transition-opacity duration-300 flex items-center justify-center">
              <div class="bg-white/90 backdrop-blur-lg w-4/5 max-w-md h-3/4 rounded-xl shadow-lg p-6"></div>
            </div>
      
            <!-- Mobile Menu Panel -->
            <div class="fixed top-0 left-0 right-0 z-50 w-full bg-white/90 backdrop-blur-lg shadow-lg rounded-b-2xl px-6 py-5 transform -translate-y-full peer-checked:translate-y-0 transition-transform duration-300 ease-in-out hidden peer-checked:flex flex-col space-y-4 lg:hidden">
              <!-- Logo & Close -->
              <div class="flex items-center justify-between">
                <a href="/project-sveltekit/">
                  <img src="assets/image/logo glint.png" alt="Logo" class="h-10 w-auto">
                </a>
                <label for="menu-toggle" class="p-2 rounded-md text-gray-700 cursor-pointer">
                  <svg class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                  </svg>
                </label>
              </div>
      
              <!-- Mobile Menu Links -->
              <nav class="flex flex-col items-start space-y-1 pt-2 text-lg">
                <a href="/project-sveltekit/" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 transition">Home</a>
      
                <!-- Products Dropdown -->
                <div class="relative w-full">
                  <input type="checkbox" id="dropdown-toggle" class="peer hidden" />
                  <div class="flex items-center -mx-2 rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
                    <a href="/project-sveltekit/product" class="flex-grow">Products</a>
                    <label for="dropdown-toggle">
                      <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
      
                <!-- Discover Us Dropdown -->
                <div class="relative w-full">
                  <input type="checkbox" id="dropdown" class="peer hidden" />
                  <div class="flex items-center -mx-2 rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
                    <a href="/project-sveltekit/#" class="flex-grow">Discover Us</a>
                    <label for="dropdown">
                      <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
          <img src="https://img.freepik.com/free-photo/young-stylist-looking-through-set-shirts-fashion-shooting_1153-5249.jpg" alt="" class="absolute inset-0 -z-10 size-full object-cover">
          <div class="absolute inset-0 -z-10 bg-black/50"></div>
      
          <div class="mx-auto max-w-7xl px-6 lg:px-8">
            <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-24 text-center">
              <div class="hidden sm:mb-8 sm:flex sm:justify-center">
                <div class="relative rounded-full px-3 py-1 text-sm/6 text-gray-400 ring-1 ring-white/10 hover:ring-white/20">
                  Kami siap membantu kebutuhan konveksi Anda.
                  <a href="/" class="font-semibold text-white">
                    <span class="absolute inset-0" aria-hidden="true"></span>Beranda <span aria-hidden="true">&rarr;</span>
                  </a>
                </div>
              </div>
              <h1 class="text-5xl font-semibold tracking-tight text-white sm:text-7xl">Hubungi Tim Glam Stitch</h1>
              <p class="mt-8 text-lg font-medium text-gray-200 sm:text-xl/8">
                Ada pertanyaan atau ingin memulai pemesanan? Kami dengan senang hati akan membantu Anda mendapatkan solusi terbaik.
              </p>
              <div class="mt-10 flex items-center justify-center gap-x-6">
                <a href="/contact" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white hover:bg-indigo-400">Hubungi Kami</a>
                <a href="/blog-list" class="text-sm/6 font-semibold text-white">Lihat Artikel <span aria-hidden="true">→</span></a>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!--end header-->
      
      <!-- contact us section -->
      <section class="bg-white py-24 sm:py-20">
          <div class="mx-auto max-w-7xl px-6 lg:px-24">
            
            <!-- Header Section -->
            <div class="text-center mb-16">
              <h2 class="text-4xl font-extrabold tracking-tight text-gray-900 sm:text-5xl mb-6">
                Butuh Bantuan? Kami Siap Membantu!
              </h2>
              <p class="text-lg text-gray-600">
                Ingin bikin kaos custom, konsultasi desain, atau sekadar tanya-tanya soal produksi? Tim <span class="font-semibold text-indigo-600">Glam Stitch</span> siap jadi partner terbaik untuk kebutuhan Anda.
              </p>
            </div>
        
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
              
              <!-- Left: Form -->
              <div>
                <form class="grid grid-cols-1 gap-y-6">
                  <div>
                    <label for="name" class="block text-sm font-medium text-gray-700">Nama Lengkap</label>
                    <input type="text" id="name" name="name" autocomplete="name"
                      class="mt-2 w-full rounded-xl border-gray-300 shadow-sm focus:border-indigo-500 focus:ring-indigo-500 px-4 py-3">
                  </div>
                  <div>
                    <label for="email" class="block text-sm font-medium text-gray-700">Email</label>
                    <input type="email" id="email" name="email" autocomplete="email"
                      class="mt-2 w-full rounded-xl border-gray-300 shadow-sm focus:border-indigo-500 focus:ring-indigo-500 px-4 py-3">
                  </div>
                  <div>
                    <label for="message" class="block text-sm font-medium text-gray-700">Pesan</label>
                    <textarea id="message" name="message" rows="4"
                      class="mt-2 w-full rounded-xl border-gray-300 shadow-sm focus:border-indigo-500 focus:ring-indigo-500 px-4 py-3"></textarea>
                  </div>
                  <div>
                    <button type="submit"
                      class="w-full inline-flex justify-center items-center rounded-xl bg-indigo-600 px-6 py-3 text-white font-semibold hover:bg-indigo-700 transition">
                      Kirim Pesan
                    </button>
                  </div>
                </form>
              </div>
        
              <!-- Right: Contact Info -->
              <div class="space-y-8">
                <div class="flex items-start gap-4">
                  <div class="flex h-16 w-16 items-center justify-center">
                    <img src="https://img.freepik.com/premium-vector/envelope-vector-illustration_1186366-13489.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Email" class="h-16 w-16 object-contain">
                  </div>
                  <div>
                    <h3 class="text-lg font-semibold text-gray-900">E-mail</h3>
                    <p><a href="/#" target="_blank" class="text-indigo-600 hover:underline">glamstitch@gmail.com</a></p>
                  </div>
                </div>
        
                <div class="flex items-start gap-4">
                  <div class="flex h-16 w-16 items-center justify-center">
                    <img src="https://img.freepik.com/premium-photo/whatsapp-logo_1080029-96.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Email" class="h-16 w-16 object-contain">
                  </div>
                  <div>
                    <h3 class="text-lg font-semibold text-gray-900">Whatsapp</h3>
                    <p><a href="/#" target="_blank" class="text-indigo-600 hover:underline">+61-882-2288-5137</a></p>
                  </div>
                </div>
        
                <div class="flex items-start gap-4">
                  <div class="flex h-16 w-16 items-center justify-center">
                    <img src="https://img.freepik.com/premium-vector/art-illustration_929495-37.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Instagram" class="h-16 w-16 object-contain">
                  </div>
                  <div>
                    <h3 class="text-lg font-semibold text-gray-900">Instagram</h3>
                    <p><a href="/https://www.instagram.com/kaospolosglamstitch/" target="_blank" class="text-indigo-600 hover:underline">@glamstitch</a></p>
                  </div>
                </div>
                <div class="space-y-8">
                  <div class="flex items-start gap-4">
                    <div class="flex h-16 w-16 items-center justify-center">
                      <img src="https://img.freepik.com/free-vector/location-pin-map-glyph_78370-1576.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Email" class="h-16 w-16 object-contain">
                    </div>
                    <div>
                      <h3 class="text-lg font-semibold text-gray-900">Lokasi</h3>
                      <p><a href="/https://maps.app.goo.gl/yofiVrQbDJmkiRkY7" target="_blank" class="text-indigo-600 hover:underline">Kabupaten Subang, Jawa Barat 41271</a></p>
                    </div>
                  </div>
              </div>
            </div>
          </div>
        </section>
      <!-- end contact us section -->
      
      <!-- FAQ Section with Image -->
      <section class="bg-white py-24 sm:py-32 relative overflow-hidden">
        <div class="absolute inset-0 -z-10 bg-gradient-to-b from-white to-gray-100"></div>
      
        <div class="max-w-7xl mx-auto px-6 lg:px-24">
          <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
            
            <!-- Left: FAQ Content -->
            <div>
              <h2 class="text-2xl font-bold tracking-tight text-gray-900 sm:text-3xl">Pertanyaan yang Sering Diajukan</h2>
              <p class="mt-2 text-base text-gray-600">Jelajahi jawaban atas pertanyaan umum mengenai layanan konveksi kami.</p>
            
              <div class="mt-8 space-y-6">
                <!-- FAQ Item -->
                <div>
                  <h3 class="text-lg font-semibold text-indigo-600">Apakah saya bisa memesan desain custom?</h3>
                  <p class="mt-1 text-sm text-gray-700">Tentu! Kirimkan desain Anda, dan tim kami akan memproduksinya dengan kualitas terbaik sesuai permintaan Anda.</p>
                </div>
            
                <div>
                  <h3 class="text-lg font-semibold text-indigo-600">Berapa minimal order?</h3>
                  <p class="mt-1 text-sm text-gray-700">Minimal pemesanan adalah 12 pcs per desain. Untuk jumlah besar, kami siap bernegosiasi harga terbaik.</p>
                </div>
            
                <div>
                  <h3 class="text-lg font-semibold text-indigo-600">Berapa lama proses produksinya?</h3>
                  <p class="mt-1 text-sm text-gray-700">Proses produksi membutuhkan waktu sekitar 7–14 hari kerja, tergantung kompleksitas desain dan jumlah pesanan.</p>
                </div>
            
                <div>
                  <h3 class="text-lg font-semibold text-indigo-600">Apakah bisa kirim ke luar kota?</h3>
                  <p class="mt-1 text-sm text-gray-700">Kami melayani pengiriman ke seluruh Indonesia dengan berbagai pilihan ekspedisi yang dapat disesuaikan.</p>
                </div>
              </div>
            
              <p class="mt-8 text-sm text-gray-700">Masih punya pertanyaan? <a href="/contact-us" class="text-indigo-600 font-medium hover:underline">Hubungi kami</a>.</p>
            </div>
            
      
            <!-- Right: Image -->
            <div class="relative rounded-xl shadow-xl overflow-hidden">
              <img src="https://img.freepik.com/free-vector/flat-people-asking-questions-illustration_23-2148910850.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Produksi Konveksi" class="w-full h-full object-cover">
              <div class="absolute inset-0 bg-indigo-600/20 mix-blend-multiply"></div>
            </div>
          </div>
        </div>
      </section>
      
      <!--end FAQ-->
      
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
              <a href="/#" class="font-semibold text-white"><span class="absolute inset-0" aria-hidden="true"></span> Lihat cerita pelanggan kami <span aria-hidden="true">&rarr;</span></a>
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
                <a href="/#" class="text-gray-500 hover:text-gray-400">
                  <span class="sr-only">Facebook</span>
                  <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                    <path d="M22 12a10 10 0 10-11.6 9.87v-6.99H8.1v-2.88h2.3V9.41c0-2.28 1.35-3.55 3.42-3.55.99 0 2.03.18 2.03.18v2.24h-1.14c-1.12 0-1.47.7-1.47 1.42v1.71h2.5l-.4 2.88h-2.1v6.99A10 10 0 0022 12z"/>
                  </svg>
                </a>
                <a href="/#" class="text-gray-500 hover:text-gray-400">
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
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Katalog Produk</a></li>
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Jasa Sablon & Bordir</a></li>
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Custom Desain Baju</a></li>
                </ul>
              </div>
              <div>
                <h3 class="text-sm font-semibold leading-6 text-white">Bantuan</h3>
                <ul role="list" class="mt-6 space-y-4">
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Cara Pemesanan</a></li>
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">FAQ</a></li>
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Hubungi Kami</a></li>
                </ul>
              </div>
              <div>
                <h3 class="text-sm font-semibold leading-6 text-white">Tentang Kami</h3>
                <ul role="list" class="mt-6 space-y-4">
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Profil Perusahaan</a></li>
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Testimoni Pelanggan</a></li>
                  <li><a href="/#" class="text-sm leading-6 text-gray-300 hover:text-white">Karir</a></li>
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
