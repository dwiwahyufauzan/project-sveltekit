<script>
    import '../../app.css';
  </script>
  
    <style type="text/tailwindcss"></style>
    <!-- Header Section -->
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

        <!-- Products Dropdown (Desktop) -->
        <div class="relative group">
          <a href="/project-sveltekit/product" class="inline-flex items-center text-lg font-semibold text-blue-400 px-3 cursor-pointer group-hover:text-blue-500 transition">
            <span>Products</span>
            <svg class="ml-2 h-5 w-5 text-blue-400 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
          <a href="/project-sveltekit/#" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 cursor-pointer group-hover:text-blue-500 transition">
            <span>Discover Us</span>
            <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
      <label for="menu-toggle" class="z-50 bg-white/80 backdrop-blur-lg p-4 rounded-full cursor-pointer lg:hidden transition-all duration-300 hover:bg-white/90">
        <svg class="w-7 h-7 text-gray-800" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </label>

      <!-- Overlay & Mobile Menu Panel -->
      <div class="fixed inset-0 z-40 bg-black/40 hidden peer-checked:block transition-opacity duration-300 lg:hidden flex items-center justify-center">
        <div class="bg-white/90 backdrop-blur-lg w-4/5 max-w-md h-3/4 rounded-xl shadow-lg p-6"></div>
      </div>

      <div class="fixed top-0 left-0 right-0 z-50 w-full bg-white/90 backdrop-blur-lg shadow-lg rounded-b-2xl px-6 py-5 transform -translate-y-full peer-checked:translate-y-0 transition-transform duration-300 ease-in-out hidden peer-checked:flex flex-col space-y-4 lg:hidden">
        <!-- Mobile Logo & Close Button -->
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

        <!-- Mobile Menu Links -->
        <nav class="flex flex-col items-start space-y-1 pt-2 text-lg">
          <a href="/project-sveltekit/" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 transition">Home</a>

          <!-- Mobile Products Dropdown -->
          <div class="relative w-full">
            <input type="checkbox" id="dropdown-toggle" class="peer hidden" />
            <div class="flex items-center -mx-2 rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
              <a href="/project-sveltekit/product" class="flex-grow">Products</a>
              <label for="dropdown-toggle">
                <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
              <a href="/project-sveltekit/#" class="flex-grow">Discover Us</a>
              <label for="dropdown">
                <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
    <img src="https://img.freepik.com/free-photo/fashionable-men-jacket-hanging-clothing-store-generated-by-ai_188544-40066.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="" class="absolute inset-0 -z-10 size-full object-cover">
    <div class="absolute inset-0 -z-10 bg-black/50"></div>

    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-24 text-center">
        <div class="hidden sm:mb-8 sm:flex sm:justify-center">
          <div class="relative rounded-full px-3 py-1 text-sm/6 text-gray-400 ring-1 ring-white/10 hover:ring-white/20">
            Eksplor pilihan jaket custom berkualitas dari Glam Stitch.
            <a href="/project-sveltekit/" class="font-semibold text-white">
              <span class="absolute inset-0" aria-hidden="true"></span>Beranda <span aria-hidden="true">&rarr;</span>
            </a>
          </div>
        </div>
        <h1 class="text-5xl font-semibold tracking-tight text-white sm:text-7xl">Produk Jaket Glam Stitch</h1>
        <p class="mt-8 text-lg font-medium text-gray-200 sm:text-xl">Temukan berbagai model jaket custom yang stylish, hangat, dan cocok untuk keperluan komunitas, kantor, hingga kebutuhan brand Anda.</p>
        <div class="mt-10 flex items-center justify-center gap-x-6">
          <a href="/project-sveltekit/contact" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-xs hover:bg-indigo-400 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-400">Pesan Sekarang</a>
          <a href="/project-sveltekit/product-list" class="text-sm font-semibold text-white">Lihat Produk Lainnya <span aria-hidden="true">→</span></a>
        </div>
      </div>
    </div>
  </div>
</div>
<!--end header-->

<!--promo sections-->
<div class="relative overflow-hidden bg-white z-0">
    <!-- Callout -->
    <section aria-labelledby="sale-heading" class="relative mx-auto flex max-w-7xl flex-col items-center px-4 pt-24 text-center sm:px-6 lg:px-8">
        <div class="mx-auto max-w-2xl lg:max-w-none">
          <h2 id="sale-heading" class="text-4xl font-bold tracking-tight text-gray-900 sm:text-5xl lg:text-5xl">
            Dapatkan Kualitas Terbaik untuk Jacket Glam Stitch Anda
          </h2>
          <p class="mx-auto mt-8 max-w-xl text-base text-gray-600">
            Sebagian besar produk kami dibuat dalam jumlah terbatas. Segera pesan Jacket Glam Stitch berkualitas tinggi sebelum habis!
          </p>
          <a href="/project-sveltekit/#" class="mt-6 inline-block w-full rounded-md border border-transparent bg-gray-900 px-8 py-3 font-medium text-white hover:bg-gray-800 sm:w-auto">
            Dapatkan Akses ke Produk Jacket Glam Stitch Kami
          </a>
        </div>
      </section>      
  </div>
<!--end promo sections-->

<!--products sections-->
<div class="bg-white">
    <main class="pt-10 sm:pt-8">
      <nav aria-label="Breadcrumb">
        <ol role="list" class="mx-auto flex max-w-2xl items-center space-x-2 px-4 sm:px-16 lg:max-w-7xl lg:px-16">
        </ol>
      </nav>
  
      <!-- Galeri Gambar -->
      <div class="mx-auto mt-6 max-w-2xl px-4 sm:px-6 lg:grid lg:max-w-7xl lg:grid-cols-3 lg:gap-x-8 lg:px-16 space-y-4 lg:space-y-0">
  
        <!-- Gambar kiri - hanya tampil di desktop -->
        <div class="hidden lg:block">
          <img src="https://media.istockphoto.com/id/1383411717/id/foto/potret-pemuda-yang-ramah.jpg?s=612x612&w=0&k=20&c=v8oJf-Volmp1s_Rt6oSzZRsKIb5GznshSDSuAH4_Dmc="
            alt="Beberapa kaos warna abu, putih, dan hitam yang diletakkan secara datar."
            class="aspect-[3/4] w-full max-w-sm mx-auto rounded-lg object-cover">
        </div>
  
        <!-- Gambar tengah (dua vertikal) - tampil di mobile -->
        <div class="grid grid-cols-1 gap-y-4">
          <img src="https://media.istockphoto.com/id/1393264537/id/foto/model-mengenakan-hoodie-pria-kulit-hitam-maket-untuk-desain-anda-sendiri.jpg?s=612x612&w=0&k=20&c=8gN8pachrbhpSFlX5VQxUDKQsvaYNk9hb69vPwr577w="
            alt="Model mengenakan kaos hitam polos."
            class="aspect-[3/2] w-full max-w-sm mx-auto rounded-lg object-cover">
          <img src="https://media.istockphoto.com/id/1438595781/id/foto/wanita-muda-berkacamata-dan-hoodie-hitam.jpg?s=612x612&w=0&k=20&c=yGm0UL4DqOxXym5Payfd1d4uSwigr-qgOCY3mHEMlrk="
            alt="Model mengenakan kaos abu polos."
            class="aspect-[3/2] w-full max-w-sm mx-auto rounded-lg object-cover">
        </div>
  
        <!-- Gambar utama -->
        <div>
          <img src="https://media.istockphoto.com/id/1366972069/id/foto/potret-pria-ceria-berkerudung-oranye.jpg?s=612x612&w=0&k=20&c=HjDQsGzANZ35dxYBk6VPK48ilGN4sXYPHA8Mwu0XRws="
            alt="Model mengenakan kaos putih polos."
            class="aspect-[4/5] w-full max-w-sm mx-auto rounded-lg object-cover lg:aspect-[3/4]">
        </div>
  
      </div>
      
      <!-- Info Produk -->
      <div class="mx-auto max-w-2xl px-4 pt-10 sm:px-6 lg:grid lg:max-w-7xl lg:grid-cols-3 lg:grid-rows-[auto_auto_1fr] lg:gap-x-8 lg:px-16 lg:pt-16">
        <div class="lg:col-span-2 lg:pr-8">
          <h1 class="text-2xl font-bold tracking-tight text-gray-900 sm:text-3xl">Jaket Glam Stitch</h1>
        </div>
      
        <!-- Opsi -->
        <div class="py-10 lg:col-span-2 lg:col-start-1 lg:pt-6 lg:pr-8 lg:pb-16">
          <!-- Deskripsi -->
          <div>
            <h3 class="sr-only">Deskripsi</h3>
            <div class="space-y-6">
              <p class="text-base text-gray-900">
                Jaket Glam Stitch hadir dengan gaya simpel dan elegan dalam tiga pilihan warna menawan. Ingin tampil berani? Pilih warna "Abu Heather". Untuk kesan premium, warna "Hitam" adalah pilihan tepat. Butuh tampilan segar dan bersih? Warna "Putih" siap menyempurnakan gayamu.
              </p>
            </div>
          </div>
      
          <!-- Highlight -->
          <div class="mt-10">
            <h3 class="text-sm font-medium text-gray-900">Fitur Unggulan</h3>
            <div class="mt-4">
              <ul role="list" class="list-disc space-y-2 pl-4 text-sm">
                <li class="text-gray-400"><span class="text-gray-600">Dijahit secara manual oleh tenaga lokal</span></li>
                <li class="text-gray-400"><span class="text-gray-600">Menggunakan pewarna eksklusif</span></li>
                <li class="text-gray-400"><span class="text-gray-600">Sudah dicuci dan disusutkan sebelumnya</span></li>
                <li class="text-gray-400"><span class="text-gray-600">100% katun super lembut</span></li>
              </ul>
            </div>
          </div>
      
          <!-- Detail Pengiriman -->
          <section aria-labelledby="shipping-heading" class="mt-10">
            <h2 id="shipping-heading" class="text-sm font-medium text-gray-900">Detail Produk</h2>
            <div class="mt-4 space-y-8">
              <p class="text-sm text-gray-600">
                Temukan produk Glam Stitch berkualitas tinggi, dirancang untuk kenyamanan dan ketahanan maksimal. Daftar sekarang untuk mendapatkan informasi warna-warna terbaru, termasuk edisi terbatas "Abu Tua" yang segera hadir.
              </p>
            </div>              
          </section>
        </div>
      </div>
      
  
      <!-- Produk Terkait -->
      <section aria-labelledby="related-products-heading" class="bg-white">
        <div class="mx-auto max-w-2xl px-16 py-24 sm:px-16 lg:max-w-7xl lg:px-16">
          <h2 id="related-products-heading" class="text-2xl font-bold tracking-tight text-gray-900 text-center">Produk Terkait</h2>
          <p class="mt-2 text-lg text-gray-400 text-center">Lihat produk Glim Stitch lainnya yang bisa kamu sukai. Tersedia berbagai pilihan stylish untuk setiap kesempatan.</p>
          <div class="mt-6 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-4 xl:gap-x-8">
      
            <!-- Produk 1 -->
            <div class="group relative">
              <img src="https://media.istockphoto.com/id/2085676478/id/foto/mockup-hoodie-putih-pada-pria-berjanggut-kaus-oversized-dengan-saku-untuk-desain-branding.jpg?s=612x612&w=0&k=20&c=7QKD-7q--IDD5CV0p5JDNuWy6f26zHLa0qCI3cF8wOc=" alt="Jaket Glim Stitch warna hitam." class="aspect-square w-full rounded-md bg-gray-200 object-cover group-hover:opacity-75 lg:aspect-auto lg:h-80">
              <div class="mt-4 flex justify-between">
                <div>
                  <h3 class="text-sm text-gray-700">
                    <a href="/project-sveltekit/#"><span aria-hidden="true" class="absolute inset-0"></span>Jaket Glim Stitch</a>
                  </h3>
                  <p class="mt-1 text-sm text-gray-500">Putih</p>
                </div>
                <p class="text-sm font-medium text-gray-900">Rp 525.000</p>
              </div>
            </div>
      
            <!-- Produk 2 -->
            <div class="group relative">
              <img src="https://media.istockphoto.com/id/2147500282/id/foto/template-hoodie-hitam-besar-pada-seorang-pria-brutal-dengan-tangan-di-saku-pakaian-lebar-untuk.jpg?s=612x612&w=0&k=20&c=O5ypltazwnlEkG_6VFkZjUN77G5hTlSzdoW5tGCnbhk=" alt="Jaket Glim Stitch warna putih." class="aspect-square w-full rounded-md bg-gray-200 object-cover group-hover:opacity-75 lg:aspect-auto lg:h-80">
              <div class="mt-4 flex justify-between">
                <div>
                  <h3 class="text-sm text-gray-700">
                    <a href="/project-sveltekit/#"><span aria-hidden="true" class="absolute inset-0"></span>Jaket Glim Stitch</a>
                  </h3>
                  <p class="mt-1 text-sm text-gray-500">Hitam</p>
                </div>
                <p class="text-sm font-medium text-gray-900">Rp 525.000</p>
              </div>
            </div>
      
            <!-- Produk 3 -->
            <div class="group relative">
              <img src="https://media.istockphoto.com/id/1314499049/id/foto/wanita-pirang-fasion-dalam-hoodie-besar-coklat-kacamata-dan-jeans-biru-mockup-untuk-logo-atau.jpg?s=612x612&w=0&k=20&c=CvvE5nL93XofC5kdnAQcVli9cB8nrOaDZvZ2vs7XhNs=" alt="Jaket Glim Stitch warna charcoal." class="aspect-square w-full rounded-md bg-gray-200 object-cover group-hover:opacity-75 lg:aspect-auto lg:h-80">
              <div class="mt-4 flex justify-between">
                <div>
                  <h3 class="text-sm text-gray-700">
                    <a href="/project-sveltekit/#"><span aria-hidden="true" class="absolute inset-0"></span>Jaket Glim Stitch</a>
                  </h3>
                  <p class="mt-1 text-sm text-gray-500">Coklat Muda</p>
                </div>
                <p class="text-sm font-medium text-gray-900">Rp 525.000</p>
              </div>
            </div>
      
            <!-- Produk 4 -->
            <div class="group relative">
              <img src="https://media.istockphoto.com/id/1652781007/id/foto/wanita-muda-tersenyum-dengan-hoodie-ungu-biru-di-mockup-ruang-copy-latar-belakang-merah-ramah.jpg?s=612x612&w=0&k=20&c=y-fN3CbRpMECwJ1epGMKPf7Ys8GAXWNoBF3xZBF-Vyo=" alt="Jaket Glim Stitch warna sienna." class="aspect-square w-full rounded-md bg-gray-200 object-cover group-hover:opacity-75 lg:aspect-auto lg:h-80">
              <div class="mt-4 flex justify-between">
                <div>
                  <h3 class="text-sm text-gray-700">
                    <a href="/project-sveltekit/#"><span aria-hidden="true" class="absolute inset-0"></span>Jaket Glim Stitch</a>
                  </h3>
                  <p class="mt-1 text-sm text-gray-500">Biru</p>
                </div>
                <p class="text-sm font-medium text-gray-900">Rp 525.000</p>
              </div>
            </div>
      
          </div>
        </div>
      </section>      
    </main>
  </div>
  
<!--end products sections-->


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
        <a href="/project-sveltekit/#" class="font-semibold text-white"><span class="absolute inset-0" aria-hidden="true"></span> Lihat cerita pelanggan kami <span aria-hidden="true">&rarr;</span></a>
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
          <a href="/project-sveltekit/#" class="text-gray-500 hover:text-gray-400">
            <span class="sr-only">Facebook</span>
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
              <path d="M22 12a10 10 0 10-11.6 9.87v-6.99H8.1v-2.88h2.3V9.41c0-2.28 1.35-3.55 3.42-3.55.99 0 2.03.18 2.03.18v2.24h-1.14c-1.12 0-1.47.7-1.47 1.42v1.71h2.5l-.4 2.88h-2.1v6.99A10 10 0 0022 12z"/>
            </svg>
          </a>
          <a href="/project-sveltekit/#" class="text-gray-500 hover:text-gray-400">
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
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Katalog Produk</a></li>
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Jasa Sablon & Bordir</a></li>
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Custom Desain Baju</a></li>
          </ul>
        </div>
        <div>
          <h3 class="text-sm font-semibold leading-6 text-white">Bantuan</h3>
          <ul role="list" class="mt-6 space-y-4">
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Cara Pemesanan</a></li>
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">FAQ</a></li>
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Hubungi Kami</a></li>
          </ul>
        </div>
        <div>
          <h3 class="text-sm font-semibold leading-6 text-white">Tentang Kami</h3>
          <ul role="list" class="mt-6 space-y-4">
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Profil Perusahaan</a></li>
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Testimoni Pelanggan</a></li>
            <li><a href="/project-sveltekit/#" class="text-sm leading-6 text-gray-300 hover:text-white">Karir</a></li>
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