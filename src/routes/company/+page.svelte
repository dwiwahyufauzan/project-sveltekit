<script>
    import '../../app.css';
  </script>
  
    <style type="text/tailwindcss"></style>
    <!-- Header -->
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
                <li><a href="/project-sveltekit/blog" class="block px-6 py-3 hover:bg-gray-100">Blog</a></li>
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
      <img src="https://img.freepik.com/premium-photo/fashion-designer-cutting-tailor-made-concept_53876-45794.jpg" alt="" class="absolute inset-0 -z-10 size-full object-cover">
      <div class="absolute inset-0 -z-10 bg-black/50"></div>
  
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-24">
          <div class="hidden sm:mb-8 sm:flex sm:justify-center">
            <div class="relative rounded-full px-3 py-1 text-sm text-gray-400 ring-1 ring-white/10 hover:ring-white/20">
              Selamat datang di Glam Stitch.
              <a href="/product" class="font-semibold text-white">
                <span class="absolute inset-0" aria-hidden="true"></span>Lihat Produk <span aria-hidden="true">&rarr;</span>
              </a>
            </div>
          </div>
          <div class="text-center">
            <h1 class="text-5xl font-semibold tracking-tight text-white sm:text-7xl">Konveksi Profesional Glam Stitch</h1>
            <p class="mt-8 text-lg font-medium text-gray-400 sm:text-xl">Kami menyediakan berbagai layanan produksi pakaian — mulai dari kaos polos, jaket custom, hingga kemeja formal — dengan standar kualitas tinggi dan pengerjaan cepat.</p>
            <div class="mt-10 flex items-center justify-center gap-x-6">
              <a href="/contact" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-400">Hubungi Kami</a>
              <a href="/portfolio" class="text-sm font-semibold text-white">Lihat Portofolio <span aria-hidden="true">→</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- End Header -->
  
  <!--hero sections-->
  <div class="relative bg-white">
    <div class="mx-auto max-w-7xl lg:grid lg:grid-cols-12 lg:gap-x-8 lg:px-16">
      
      <!-- Kiri: Teks -->
      <div class="px-6 pt-10 pb-24 sm:pb-32 lg:col-span-7 lg:px-0 lg:pt-40 lg:pb-16 xl:col-span-6 flex items-center">
        <div class="mx-auto max-w-lg lg:mx-0">
          <div class="hidden sm:mt-32 sm:flex lg:mt-16">
            <div class="relative rounded-full px-3 py-1 text-sm/6 text-gray-500 ring-1 ring-gray-900/10 hover:ring-gray-900/20">
              Kami bangga melayani berbagai klien dengan produk pakaian berkualitas tinggi.
              <a href="/#" class="font-semibold whitespace-nowrap text-indigo-600">
                <span class="absolute inset-0" aria-hidden="true"></span>
                Temukan lebih lanjut <span aria-hidden="true">&rarr;</span>
              </a>
            </div>
          </div>
          <h1 class="mt-24 text-5xl font-semibold tracking-tight text-pretty text-gray-900 sm:mt-10 sm:text-7xl">
            Glam Stitch Konveksi Profesional
          </h1>
          <p class="mt-8 text-lg font-medium text-pretty text-gray-500 sm:text-xl/8">
            Glam Stitch adalah penyedia solusi pakaian kustom untuk berbagai kebutuhan bisnis, organisasi, dan acara. Kami siap memenuhi pesanan seragam, merchandise, atau pakaian promosi dengan hasil berkualitas tinggi yang disesuaikan dengan kebutuhan Anda.
          </p>
          <div class="mt-10 flex items-center gap-x-6">
            <a href="/#services" class="rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-xs hover:bg-indigo-500 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Layanan Kami</a>
            <a href="/#about" class="text-sm/6 font-semibold text-gray-900">Pelajari lebih lanjut <span aria-hidden="true">→</span></a>
          </div>
        </div>
      </div>
  
      <!-- Kanan: Gambar -->
      <div class="relative lg:col-span-5 lg:-mr-8 xl:absolute xl:inset-0 xl:left-1/2 xl:mr-0 flex items-center justify-center h-full">
        <img
          class="w-full max-w-xs sm:max-w-sm md:max-w-md lg:max-w-md xl:max-w-lg mt-10 bg-gray-900 object-contain rounded-2xl"
          src="assets/image/logo glint.png"
          alt="logo glam stitch"
        >
      </div>
      
      
    </div>
  </div>
  <!--end hero sections-->
  
  <!--content-->
  <div class="bg-white py-24">
    <div class="mx-auto max-w-7xl px-6 lg:px-16">
      <div class="mx-auto flex max-w-2xl flex-col items-center justify-between gap-8 lg:mx-0 lg:max-w-none lg:flex-row lg:items-center">
        
        <!-- Gambar -->
        <div class="w-full lg:max-w-lg lg:flex-auto">
          <img src="https://media.istockphoto.com/id/1477822155/id/foto/tim-bisnis-yang-sukses-terhubung-dengan-klien-mereka-melalui-panggilan-video.jpg?s=612x612&w=0&k=20&c=5huRlrTzfFkLe7jsttX6RgeCjoRvuz5N7ywpef5tlww=" class="w-full rounded-2xl bg-gray-50 object-cover" alt="Gambar Konveksi">
        </div>
  
        <!-- Teks -->
        <div class="w-full lg:max-w-xl lg:flex-auto">
          <h3 class="sr-only">Visi, Misi, dan Nilai</h3>
          <ul class="mt-6 space-y-4 text-gray-600 list-disc list-inside text-base/7">
            <li>
              <strong>Visi:</strong> Menjadi pemimpin terkemuka dalam industri konveksi yang dikenal akan kualitas unggul, inovasi, dan kepuasan pelanggan.
            </li>
            <li>
              <strong>Misi 1:</strong> Memberikan pakaian kustom berkualitas tinggi sesuai kebutuhan pelanggan dengan menerapkan praktik produksi yang berkelanjutan.
            </li>
            <li>
              <strong>Misi 2:</strong> Membangun hubungan jangka panjang dengan klien melalui layanan yang andal, inovatif, dan berfokus pada kepuasan pelanggan.
            </li>
            <li>
              <strong>Komitmen Kualitas:</strong> Kami percaya bahwa setiap pakaian harus dibuat dengan ketelitian dan standar tertinggi.
            </li>
            <li>
              <strong>Inovasi:</strong> Kami mengadopsi teknologi dan teknik terbaru untuk meningkatkan kemampuan produksi dan menciptakan solusi pakaian yang modern.
            </li>
            <li>
              <strong>Keberlanjutan:</strong> Glam Stitch berkomitmen mengurangi dampak lingkungan dengan menerapkan praktik produksi yang ramah lingkungan.
            </li>
          </ul>
        </div>
  
      </div>
    </div>
  </div>
  <!--end content-->
  
  <!-- our journey -->
  <section class="bg-white py-20" id="our-journey">
    <div class="mx-auto max-w-7xl px-6 lg:px-16">
      <div class="text-center mb-16">
        <h2 class="text-4xl font-bold text-gray-800">Perjalanan Kami</h2>
        <p class="mt-4 text-lg text-gray-600">Langkah-langkah penting Glam Stitch dari awal hingga kini.</p>
      </div>
  
      <div class="space-y-16 relative border-l-4 border-indigo-500 pl-8">
        <!-- 2020 -->
        <div class="relative">
          <div class="absolute -left-5 top-1 w-10 h-10 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold shadow-md">2020</div>
          <div class="grid grid-cols-1 md:grid-cols-2 items-center gap-6">
            <img src="https://img.freepik.com/premium-photo/tailors-shop-with-equipment-work-benches_126745-1092.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="2020" class="rounded-xl shadow-lg w-full h-64 object-cover">
            <p class="text-gray-700 text-lg">
              Awal mula berdirinya Glam Stitch, dimulai dari sebuah rumah kecil di Cijoged dengan mesin jahit sederhana dan semangat besar untuk memberikan kualitas terbaik.
            </p>
          </div>
        </div>
  
        <!-- 2021 -->
        <div class="relative">
          <div class="absolute -left-5 top-1 w-10 h-10 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold shadow-md">2021</div>
          <div class="grid grid-cols-1 md:grid-cols-2 items-center gap-6">
            <img src="https://img.freepik.com/free-photo/woman-business-owner-working-her-tailor-shop_1150-11672.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="2021" class="rounded-xl shadow-lg w-full h-64 object-cover">
            <p class="text-gray-700 text-lg">
              Memperluas layanan dengan mulai menerima pesanan dalam jumlah besar dari komunitas dan sekolah. Glam Stitch mulai dikenal di wilayah lokal.
            </p>
          </div>
        </div>
  
        <!-- 2022 -->
        <div class="relative">
          <div class="absolute -left-5 top-1 w-10 h-10 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold shadow-md">2022</div>
          <div class="grid grid-cols-1 md:grid-cols-2 items-center gap-6">
            <img src="https://img.freepik.com/free-photo/portrait-businesswoman-owner_23-2148828328.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="2022" class="rounded-xl shadow-lg w-full h-64 object-cover">
            <p class="text-gray-700 text-lg">
              Tahun inovasi. Kami memperkenalkan layanan custom desain dan menambah 5 mesin jahit industri untuk meningkatkan kapasitas produksi.
            </p>
          </div>
        </div>
  
        <!-- 2023 -->
        <div class="relative">
          <div class="absolute -left-5 top-1 w-10 h-10 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold shadow-md">2023</div>
          <div class="grid grid-cols-1 md:grid-cols-2 items-center gap-6">
            <img src="https://img.freepik.com/free-vector/organic-flat-blog-post-illustration-with-people_23-2148955260.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="2023" class="rounded-xl shadow-lg w-full h-64 object-cover">
            <p class="text-gray-700 text-lg">
              Glam Stitch meluncurkan website resmi dan menjangkau pelanggan dari seluruh Indonesia. Jaringan reseller pun mulai dibentuk.
            </p>
          </div>
        </div>
  
        <!-- 2024 -->
        <div class="relative">
          <div class="absolute -left-5 top-1 w-10 h-10 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold shadow-md">2024</div>
          <div class="grid grid-cols-1 md:grid-cols-2 items-center gap-6">
            <img src="https://img.freepik.com/free-vector/new-employee-concept-illustration_114360-7805.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="2024" class="rounded-xl shadow-lg w-full h-64 object-cover">
            <p class="text-gray-700 text-lg">
              Kini Glam Stitch telah menjadi konveksi terpercaya dengan lebih dari 100 klien aktif. Kami terus berkomitmen memberikan pelayanan terbaik.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- end our journey -->
  
  
  
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
  <!--end footers-->