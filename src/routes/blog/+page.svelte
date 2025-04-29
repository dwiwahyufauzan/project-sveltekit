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
          <img src="assets/image/logo glint.png" alt="Your Company Logo" class="h-14 w-14 object-contain">
        </a>
  
        <!-- Desktop Menu -->
        <div class="hidden lg:flex lg:gap-x-8">
          <a href="/project-sveltekit/" class="text-lg font-semibold text-gray-900">Home</a>
  
          <!-- Products Dropdown (Desktop) -->
          <div class="relative group">
            <a href="/project-sveltekit/product" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 cursor-pointer group-hover:text-blue-500 transition">
              <span>Products</span>
              <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
  
          <!-- Discover Us Dropdown (Desktop) -->
          <div class="relative group">
            <a href="/project-sveltekit/#" class="inline-flex items-center text-lg font-semibold text-blue-400 px-3 cursor-pointer group-hover:text-blue-500 transition">
              <span>Discover Us</span>
              <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
              </svg>
            </a>
            <div class="absolute left-0 mt-2 w-52 bg-white shadow-lg rounded-lg z-50 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-200 ease-in-out">
              <ul class="py-2 text-lg text-gray-700">
                <li><a href="/project-sveltekit/company" class="block px-6 py-3 hover:bg-gray-100">About Us</a></li>
                <li><a href="/project-sveltekit/project-sveltekit/blog" class="block px-6 py-3 hover:bg-gray-100">Blog</a></li>
                <li><a href="/project-sveltekit/contact-us" class="block px-6 py-3 hover:bg-gray-100">Contact Us</a></li>
                <li><a href="/project-sveltekit/lokasi" class="block px-6 py-3 hover:bg-gray-100">Store Location</a></li>
              </ul>
            </div>
          </div>
        </div>
  
        <!-- Mobile Hamburger Menu -->
        <input type="checkbox" id="menu-toggle" class="peer hidden" />
        <label for="menu-toggle" class="z-50 bg-white/80 backdrop-blur-lg p-4 rounded-full cursor-pointer lg:hidden transition-all duration-300 hover:bg-white/90">
          <svg class="w-7 h-7 text-gray-800" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </label>
  
        <!-- Mobile Overlay -->
        <div class="fixed inset-0 z-40 bg-black/40 hidden peer-checked:block transition-opacity duration-300 lg:hidden flex items-center justify-center">
          <div class="bg-white/90 backdrop-blur-lg w-4/5 max-w-md h-3/4 rounded-xl shadow-lg p-6">
            <!-- Optional content here -->
          </div>
        </div>
  
        <!-- Mobile Menu -->
        <div class="fixed top-0 left-0 right-0 z-50 w-full bg-white/90 backdrop-blur-lg shadow-lg rounded-b-2xl px-6 py-5 transform -translate-y-full peer-checked:translate-y-0 transition-transform duration-300 ease-in-out hidden peer-checked:flex flex-col space-y-4 lg:hidden">
          <div class="flex items-center justify-between">
            <a href="/project-sveltekit/"><img src="assets/image/logo glint.png" alt="Logo" class="h-10 w-auto"></a>
            <label for="menu-toggle" class="p-2 rounded-md text-gray-700 cursor-pointer">
              <svg class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
              </svg>
            </label>
          </div>
  
          <nav class="flex flex-col items-start space-y-1 pt-2 text-lg">
            <a href="/project-sveltekit/" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 transition">Home</a>
  
            <!-- Products Mobile Dropdown -->
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
  
            <!-- Discover Us Mobile Dropdown -->
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
      <img src="https://img.freepik.com/free-photo/close-up-image-lot-coils-with-threads-sewing-workshop_613910-19021.jpg?w=740" alt="Background" class="absolute inset-0 -z-10 w-full h-full object-cover">
      <div class="absolute inset-0 -z-10 bg-black/50"></div>
  
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-24 text-center">
          <div class="hidden sm:mb-8 sm:flex sm:justify-center">
            <div class="relative rounded-full px-3 py-1 text-sm text-gray-400 ring-1 ring-white/10 hover:ring-white/20">
              Dapatkan inspirasi dan informasi terbaru seputar dunia konveksi.
              <a href="/" class="font-semibold text-white">Beranda <span aria-hidden="true">&rarr;</span></a>
            </div>
          </div>
          <h1 class="text-5xl font-semibold tracking-tight text-white sm:text-7xl">Blog Glam Stitch</h1>
          <p class="mt-8 text-lg font-medium text-gray-400 sm:text-xl">
            Temukan artikel menarik tentang tren fashion, tips produksi pakaian, hingga cerita di balik layar Glam Stitch.
          </p>
          <div class="mt-10 flex items-center justify-center gap-x-6">
            <a href="/blog-list" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white hover:bg-indigo-400">Lihat Artikel</a>
            <a href="/contact" class="text-sm font-semibold text-white">Hubungi Kami <span aria-hidden="true">&rarr;</span></a>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!--end header-->
  
  <!--blog sections-->
  <section class="bg-gradient-to-b from-gray-50 via-white to-white py-24 sm:py-20">
    <div class="mx-auto max-w-7xl px-6 lg:px-16">
      <div class="mx-auto max-w-2xl text-center">
        <h2 class="text-4xl font-bold text-gray-900 sm:text-5xl tracking-wide">Artikel & Cerita dari Glam Stitch</h2>
        <p class="mt-4 text-lg text-gray-600">Temukan wawasan menarik, kisah inspiratif, dan tips bermanfaat seputar dunia konveksi serta perkembangan bisnis kami.</p>
      </div>
  
      <div class="mt-16 grid grid-cols-1 gap-8 sm:grid-cols-2 lg:grid-cols-3">
        <!-- Post 1 -->
        <article class="rounded-2xl overflow-hidden bg-white shadow-lg hover:shadow-2xl transition-shadow duration-300 transform hover:scale-105">
          <img src="https://media.istockphoto.com/id/1269798844/id/foto/terinspirasi-wanita-muda-asia-ide-bagus.jpg?s=612x612&w=0&k=20&c=dpoO_SJ-ZOf5LDfS89333lsqYz0KFVbRPduB8pnvrk0=" alt="Produksi Kaos Polos" class="w-full h-64 object-cover rounded-t-2xl transition-transform duration-500 ease-in-out transform hover:scale-110">
          <div class="p-6">
            <time datetime="2025-04-15" class="text-sm text-indigo-500">15 April 2025</time>
            <h3 class="mt-2 text-xl font-semibold text-gray-900 hover:text-indigo-600 transition-all duration-200">Di Balik Produksi Kaos Polos Kami</h3>
            <p class="mt-2 text-gray-600">Intip proses produksi yang kami jalankan untuk menghadirkan kaos polos berkualitas premium dan nyaman digunakan.</p>
            <a href="/#" class="mt-4 inline-block text-sm font-semibold text-indigo-600 hover:text-indigo-500">Baca Selengkapnya →</a>
          </div>
        </article>
  
        <!-- Post 2 -->
        <article class="rounded-2xl overflow-hidden bg-white shadow-lg hover:shadow-2xl transition-shadow duration-300 transform hover:scale-105">
          <img src="https://media.istockphoto.com/id/2042011981/id/foto/male-african-american-tailor-is-making-a-sketch-in-his-atelier.jpg?s=612x612&w=0&k=20&c=htWFYHyrCnyVXSy3dL3EbtjfJessNbNuG_uFhDE4eUk=" alt="Tips Bahan Kaos" class="w-full h-64 object-cover rounded-t-2xl transition-transform duration-500 ease-in-out transform hover:scale-110">
          <div class="p-6">
            <time datetime="2025-04-10" class="text-sm text-indigo-500">10 April 2025</time>
            <h3 class="mt-2 text-xl font-semibold text-gray-900 hover:text-indigo-600 transition-all duration-200">Panduan Memilih Bahan Terbaik</h3>
            <p class="mt-2 text-gray-600">Mau produksi kaos tapi bingung pilih bahan? Kami bantu Anda memahami perbedaan bahan dan penggunaannya.</p>
            <a href="/#" class="mt-4 inline-block text-sm font-semibold text-indigo-600 hover:text-indigo-500">Baca Selengkapnya →</a>
          </div>
        </article>
  
        <!-- Post 3 -->
        <article class="rounded-2xl overflow-hidden bg-white shadow-lg hover:shadow-2xl transition-shadow duration-300 transform hover:scale-105">
          <img src="https://media.istockphoto.com/id/1215557826/id/foto/proses-produksi-tangan-laki-laki-bekerja-dengan-sketsa-atau-pola-di-studio-dan-menyiapkan-kain.jpg?s=612x612&w=0&k=20&c=AB8HCVta2oIWY_Rs0tdvepwHoT79p0Cogsgi6us0PDs=" alt="Konveksi Lokal" class="w-full h-64 object-cover rounded-t-2xl transition-transform duration-500 ease-in-out transform hover:scale-110">
          <div class="p-6">
            <time datetime="2025-04-05" class="text-sm text-indigo-500">5 April 2025</time>
            <h3 class="mt-2 text-xl font-semibold text-gray-900 hover:text-indigo-600 transition-all duration-200">Kekuatan UMKM Lokal: Cerita dari Cijoged</h3>
            <p class="mt-2 text-gray-600">Glam Stitch tumbuh bersama komunitas lokal. Inilah alasan kami bangga menjadi bagian dari konveksi lokal di Cijoged.</p>
            <a href="/#" class="mt-4 inline-block text-sm font-semibold text-indigo-600 hover:text-indigo-500">Baca Selengkapnya →</a>
          </div>
        </article>
      </div>
    </div>
  </section>
  <!--end blog sec-->
  
  
  <!--testimonial sections-->
  <div class="bg-white py-24 sm:py-16">
    <div class="mx-auto max-w-7xl px-6 lg:px-16">
      <div class="mx-auto max-w-2xl text-center">
        <h2 class="mt-2 text-4xl font-semibold tracking-tight text-balance text-gray-900 sm:text-5xl">
          Testimoni Klien Konveksi Glam Stitch
        </h2>
        <p class="mt-4 text-lg text-gray-600">Dipercaya oleh berbagai brand dan bisnis yang puas dengan hasil produksi kami.</p>
      </div>
      <div class="mx-auto mt-16 flow-root max-w-2xl sm:mt-20 lg:mx-0 lg:max-w-none">
        <div class="-mt-8 sm:-mx-4 sm:columns-2 sm:text-[0] lg:columns-3">
          
          <!-- Testimoni 1 -->
          <div class="pt-8 sm:inline-block sm:w-full sm:px-4">
            <figure class="rounded-2xl bg-gray-50 p-8 text-sm/6">
              <blockquote class="text-gray-900">
                <p>“Kualitas bahan dan jahitan sangat bagus. Pesanan kaos promosi kami selesai tepat waktu dan hasilnya memuaskan.”</p>
              </blockquote>
              <figcaption class="mt-6 flex items-center gap-x-4">
                <img class="size-10 rounded-full" src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                <div>
                  <div class="font-semibold text-gray-900">Putri Aulia</div>
                  <div class="text-gray-600">@putriaulia</div>
                </div>
              </figcaption>
            </figure>
          </div>
  
          <!-- Testimoni 2 -->
          <div class="pt-8 sm:inline-block sm:w-full sm:px-4">
            <figure class="rounded-2xl bg-gray-50 p-8 text-sm/6">
              <blockquote class="text-gray-900">
                <p>“Pelayanan cepat dan responsif. Jaket kantor yang kami pesan hasilnya rapi dan profesional.”</p>
              </blockquote>
              <figcaption class="mt-6 flex items-center gap-x-4">
                <img class="size-10 rounded-full" src="https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                <div>
                  <div class="font-semibold text-gray-900">Rahmat Hidayat</div>
                  <div class="text-gray-600">@rahmathdy</div>
                </div>
              </figcaption>
            </figure>
          </div>
  
          <!-- Testimoni 3 -->
          <div class="pt-8 sm:inline-block sm:w-full sm:px-4">
            <figure class="rounded-2xl bg-gray-50 p-8 text-sm/6">
              <blockquote class="text-gray-900">
                <p>“Sangat perhatian terhadap detail. Kaos komunitas kami dibuat sesuai desain dan ukuran yang kami inginkan.”</p>
              </blockquote>
              <figcaption class="mt-6 flex items-center gap-x-4">
                <img class="size-10 rounded-full" src="https://images.unsplash.com/photo-1544723795-3fb6469f5b39?auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                <div>
                  <div class="font-semibold text-gray-900">Melati Nurfadila</div>
                  <div class="text-gray-600">@melatinur</div>
                </div>
              </figcaption>
            </figure>
          </div>
  
          <!-- Testimoni 4 -->
          <div class="pt-8 sm:inline-block sm:w-full sm:px-4">
            <figure class="rounded-2xl bg-gray-50 p-8 text-sm/6">
              <blockquote class="text-gray-900">
                <p>“Hasil bordirnya detail dan rapi. Kami sangat puas dengan seragam kerja yang dibuat oleh Glam Stitch.”</p>
              </blockquote>
              <figcaption class="mt-6 flex items-center gap-x-4">
                <img class="size-10 rounded-full" src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                <div>
                  <div class="font-semibold text-gray-900">Daniel Surya</div>
                  <div class="text-gray-600">@danielsurya</div>
                </div>
              </figcaption>
            </figure>
          </div>
  
          <!-- Testimoni 5 -->
          <div class="pt-8 sm:inline-block sm:w-full sm:px-4">
            <figure class="rounded-2xl bg-gray-50 p-8 text-sm/6">
              <blockquote class="text-gray-900">
                <p>“Order kaos event kami diproses sangat cepat dan hasil sablonnya tajam. Terima kasih Glam Stitch!”</p>
              </blockquote>
              <figcaption class="mt-6 flex items-center gap-x-4">
                <img class="size-10 rounded-full" src="https://images.unsplash.com/photo-1517365830460-955ce3ccd263?auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                <div>
                  <div class="font-semibold text-gray-900">Alya Ramadhani</div>
                  <div class="text-gray-600">@alyaram</div>
                </div>
              </figcaption>
            </figure>
          </div>
  
          <!-- Testimoni 6 -->
          <div class="pt-8 sm:inline-block sm:w-full sm:px-4">
            <figure class="rounded-2xl bg-gray-50 p-8 text-sm/6">
              <blockquote class="text-gray-900">
                <p>“Timnya sangat kooperatif. Kami bisa request desain khusus dan hasilnya sangat memuaskan. Recommended!”</p>
              </blockquote>
              <figcaption class="mt-6 flex items-center gap-x-4">
                <img class="size-10 rounded-full" src="https://images.unsplash.com/photo-1463453091185-61582044d556?auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                <div>
                  <div class="font-semibold text-gray-900">Farhan Naufal</div>
                  <div class="text-gray-600">@farhannfl</div>
                </div>
              </figcaption>
            </figure>
          </div>
  
        </div>
      </div>
    </div>
  </div>
  <!--end testimonial sections-->
  
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