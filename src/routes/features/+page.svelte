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
              <img class="h-14 w-14 object-contain" src="assets/image/logo glint.png" alt="Your Company Logo">
            </a>
      
            <!-- Desktop Menu -->
            <div class="hidden lg:flex lg:gap-x-8">
              <a href="/" class="text-lg font-semibold text-gray-900">Home</a>
      
              <!-- Products Dropdown (Desktop) -->
              <div class="relative group">
                <a href="/product" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 cursor-pointer group-hover:text-blue-500 transition">
                  <span>Products</span>
                  <svg class="ml-2 h-5 w-5 text-gray-900 group-hover:text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
      
              <a href="/features" class="text-lg font-semibold text-blue-400">Services</a>
      
              <!-- Discover Us Dropdown (Desktop) -->
              <div class="relative group">
                <a href="/#" class="inline-flex items-center text-lg font-semibold text-gray-900 px-3 cursor-pointer group-hover:text-blue-500 transition">
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
            <input type="checkbox" id="menu-toggle" class="peer hidden" autocomplete="off" />
            <label for="menu-toggle" class="z-50 bg-white/80 backdrop-blur-lg p-4 rounded-full cursor-pointer lg:hidden transition-all duration-300 hover:bg-white/90">
              <svg class="w-7 h-7 text-gray-800" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
              </svg>
            </label>
      
            <!-- Mobile Menu Overlay -->
            <div class="fixed inset-0 z-40 bg-black/40 hidden peer-checked:block transition-opacity duration-300 lg:hidden flex items-center justify-center">
              <div class="bg-white/90 backdrop-blur-lg w-4/5 max-w-md h-3/4 rounded-xl shadow-lg p-6"></div>
            </div>
      
            <!-- Mobile Menu Panel -->
            <div class="fixed top-0 left-0 right-0 z-50 w-full bg-white/90 backdrop-blur-lg shadow-lg rounded-b-2xl px-6 py-5 transform -translate-y-full peer-checked:translate-y-0 transition-transform duration-300 ease-in-out hidden peer-checked:flex flex-col space-y-4 lg:hidden">
              <div class="flex items-center justify-between">
                <a href="/"><img src="assets/image/logo glint.png" alt="Logo" class="h-10 w-auto"></a>
                <label for="menu-toggle" class="p-2 rounded-md text-gray-700 cursor-pointer">
                  <svg class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                  </svg>
                </label>
              </div>
      
              <!-- Mobile Menu Links -->
              <nav class="flex flex-col items-start space-y-1 pt-2 text-lg">
                <a href="/" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 transition">Home</a>
      
                <!-- Products Dropdown (Mobile) -->
                <div class="relative w-full">
                  <input type="checkbox" id="dropdown-toggle" class="peer hidden" />
                  <div class="flex items-center -mx-2 rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
                    <a href="/product" class="flex-grow">Products</a>
                    <label for="dropdown-toggle">
                      <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
      
                <a href="/features" class="-mx-2 block rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 transition">Services</a>
      
                <!-- Discover Us Dropdown (Mobile) -->
                <div class="relative w-full">
                  <input type="checkbox" id="dropdown" class="peer hidden" />
                  <div class="flex items-center -mx-2 rounded-md px-3 py-1.5 font-medium text-gray-900 hover:bg-gray-50 justify-between cursor-pointer">
                    <a href="/#" class="flex-grow">Discover Us</a>
                    <label for="dropdown">
                      <svg class="h-4 w-4 text-gray-800 transition-transform peer-checked:rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
          <img src="https://img.freepik.com/free-photo/close-up-people-with-tablet_23-2149196087.jpg" alt="" class="absolute inset-0 -z-10 size-full object-cover">
          <div class="absolute inset-0 -z-10 bg-black/50"></div>
      
          <div class="mx-auto max-w-7xl px-6 lg:px-8">
            <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-24">
              <div class="hidden sm:mb-8 sm:flex sm:justify-center">
                <div class="relative rounded-full px-3 py-1 text-sm/6 text-gray-400 ring-1 ring-white/10 hover:ring-white/20">
                  Solusi konveksi terbaik untuk kebutuhan Anda.
                  <a href="/product" class="font-semibold text-white">
                    <span class="absolute inset-0" aria-hidden="true"></span>Lihat Produk <span aria-hidden="true">&rarr;</span>
                  </a>
                </div>
              </div>
              <div class="text-center">
                <h1 class="text-5xl font-semibold tracking-tight text-balance text-white sm:text-7xl">
                  Layanan Konveksi Profesional dari Glam Stitch
                </h1>
                <p class="mt-8 text-lg font-medium text-pretty text-gray-400 sm:text-xl/8">
                  Kami menyediakan berbagai layanan produksi pakaian — mulai dari kaos polos, jaket custom, hingga kemeja formal — dengan standar kualitas tinggi dan pengerjaan cepat.
                </p>
                <div class="mt-10 flex items-center justify-center gap-x-6">
                  <a href="/contact" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-xs hover:bg-indigo-400 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-400">Hubungi Kami</a>
                  <a href="/portfolio" class="text-sm/6 font-semibold text-white">Lihat Portofolio <span aria-hidden="true">→</span></a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!--end header-->
      
      <!--cta-->
      <section class="py-24 bg-gradient-to-br from-white bg-white">
        <div class="max-w-7xl mx-auto px-6 lg:px-16">
          <div class="text-center mb-16">
            <h2 class="text-4xl font-extrabold text-gray-800 sm:text-5xl tracking-wide">Layanan Unggulan Glam Stitch</h2>
            <p class="mt-4 text-lg text-gray-600">Nikmati layanan bordir, sablon, dan custom desain yang elegan, cepat, dan sesuai identitas brand Anda.</p>
          </div>
      
          <div class="grid grid-cols-1 md:grid-cols-3 gap-10">
            <!-- Jasa Bordir -->
            <div class="group bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl hover:-translate-y-1 transition duration-300">
              <div class="relative overflow-hidden rounded-2xl mb-6">
                <img src="https://img.freepik.com/free-photo/portrait-businesswoman-owner_23-2148828328.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Jasa Bordir" class="w-full h-60 object-cover rounded-2xl group-hover:scale-105 transition duration-500">
                <div class="absolute top-4 left-4 bg-blue-600 text-white text-sm font-semibold px-3 py-1 rounded-full">Bordir</div>
              </div>
              <h3 class="text-2xl font-bold text-gray-800 mb-2">Jasa Bordir Profesional</h3>
              <p class="text-gray-600 mb-4">Tingkatkan identitas brand Anda dengan hasil bordir presisi, tahan lama, dan elegan untuk segala kebutuhan.</p>
              <a href="/#" class="inline-flex items-center gap-2 text-blue-600 font-semibold hover:text-blue-400 transition text-sm">
                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M17 8l4 4m0 0l-4 4m4-4H3"/></svg>
                Pelajari Lebih Lanjut
              </a>
              <div class="mt-6">
                <button class="bg-blue-600 text-white font-semibold px-5 py-2 rounded-xl hover:bg-blue-700 transition">Pesan Sekarang</button>
              </div>
            </div>
      
            <!-- Jasa Sablon -->
            <div class="group bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl hover:-translate-y-1 transition duration-300">
              <div class="relative overflow-hidden rounded-2xl mb-6">
                <img src="https://img.freepik.com/premium-photo/close-up-person-working-textile-industry_1048944-24648174.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Jasa Sablon" class="w-full h-60 object-cover rounded-2xl group-hover:scale-105 transition duration-500">
                <div class="absolute top-4 left-4 bg-blue-600 text-white text-sm font-semibold px-3 py-1 rounded-full">Sablon</div>
              </div>
              <h3 class="text-2xl font-bold text-gray-800 mb-2">Sablon Kaos Berkualitas</h3>
              <p class="text-gray-600 mb-4">Layanan sablon dengan hasil warna tajam dan tahan lama, cocok untuk kaos komunitas, promosi, hingga distro.</p>
              <a href="/#" class="inline-flex items-center gap-2 text-blue-600 font-semibold hover:text-blue-400 transition text-sm">
                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M17 8l4 4m0 0l-4 4m4-4H3"/></svg>
                Pelajari Lebih Lanjut
              </a>
              <div class="mt-6">
                <button class="bg-blue-600 text-white font-semibold px-5 py-2 rounded-xl hover:bg-blue-700 transition">Cek Harga</button>
              </div>
            </div>
      
            <!-- Custom Desain Baju -->
            <div class="group bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl hover:-translate-y-1 transition duration-300">
              <div class="relative overflow-hidden rounded-2xl mb-6">
                <img src="https://img.freepik.com/free-photo/drawing-fabric_1098-18012.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Custom Desain Baju" class="w-full h-60 object-cover rounded-2xl group-hover:scale-105 transition duration-500">
                <div class="absolute top-4 left-4 bg-blue-600 text-white text-sm font-semibold px-3 py-1 rounded-full">Custom</div>
              </div>
              <h3 class="text-2xl font-bold text-gray-800 mb-2">Custom Desain Baju</h3>
              <p class="text-gray-600 mb-4">Bebaskan kreativitasmu! Bekerja sama dengan tim desain kami untuk menciptakan pakaian yang unik.</p>
              <a href="/#" class="inline-flex items-center gap-2 text-blue-600 font-semibold hover:text-blue-400 transition text-sm">
                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M17 8l4 4m0 0l-4 4m4-4H3"/></svg>
                Pelajari Lebih Lanjut
              </a>
              <div class="mt-6">
                <button class="bg-blue-600 text-white font-semibold px-5 py-2 rounded-xl hover:bg-blue-700 transition">Konsultasi Desain</button>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!--end cta-->
      
      <!--features-->
      <div class="bg-gray-100">
        <div class="relative mx-auto max-w-7xl px-4 pt-16 pb-16 sm:px-6 lg:px-32">
          <dl class="mx-auto grid max-w-2xl grid-cols-1 gap-6 sm:grid-cols-2 lg:max-w-none lg:grid-cols-3">
            
            <!-- Asal Produksi -->
            <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition-all duration-300">
              <dt class="text-lg font-semibold text-gray-900">Buatan Sendiri</dt>
              <dd class="mt-2 text-gray-600 text-sm">Semua produk dikerjakan langsung di workshop kami oleh tim ahli, bukan outsourcing.</dd>
            </div>
      
            <!-- Bahan -->
            <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition-all duration-300">
              <dt class="text-lg font-semibold text-gray-900">Bahan Premium</dt>
              <dd class="mt-2 text-gray-600 text-sm">Kami gunakan kain terbaik seperti Cotton Combed, Polyester, dan Drill. Lembut dan awet.</dd>
            </div>
      
            <!-- Ukuran -->
            <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition-all duration-300">
              <dt class="text-lg font-semibold text-gray-900">Ukuran Lengkap</dt>
              <dd class="mt-2 text-gray-600 text-sm">Tersedia semua ukuran dari XS sampai XXL. Bisa juga custom sesuai permintaan.</dd>
            </div>
      
            <!-- Finishing -->
            <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition-all duration-300">
              <dt class="text-lg font-semibold text-gray-900">Finishing Rapi</dt>
              <dd class="mt-2 text-gray-600 text-sm">Setiap produk dijahit dengan rapi dan dicek ulang sebelum dikirim.</dd>
            </div>
      
            <!-- Paket -->
            <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition-all duration-300">
              <dt class="text-lg font-semibold text-gray-900">Semua Sudah Termasuk</dt>
              <dd class="mt-2 text-gray-600 text-sm">Mulai dari desain, potong, jahit, sampai packing—semuanya sudah termasuk.</dd>
            </div>
      
            <!-- Catatan -->
            <div class="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition-all duration-300">
              <dt class="text-lg font-semibold text-gray-900">Catatan Penting</dt>
              <dd class="mt-2 text-gray-600 text-sm">Warna kain bisa sedikit beda karena layar & bahan. Tapi kami selalu jaga kualitas terbaik.</dd>
            </div>
      
          </dl>
        </div>
      </div>
      
      <!--end features-->
      
      <!-- Jam Kerja -->
      <section class="bg-white py-12 sm:py-16">
        <div class="mx-auto max-w-7xl px-6 lg:px-16">
          <div class="text-center">
            <h2 class="text-3xl font-extrabold text-gray-900 sm:text-4xl">
              Jam Kerja Kami
            </h2>
            <p class="mt-4 text-lg text-gray-600">
              Kami siap membantu Anda sesuai dengan jam kerja yang terjadwal di bawah ini.
            </p>
          </div>
          <div class="mt-10 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Senin - Jumat -->
            <div class="flex justify-center items-center bg-white rounded-xl shadow-md p-6">
              <div class="text-center">
                <img src="https://media.istockphoto.com/id/1283403359/id/vektor/ikon-waktu-di-latar-belakang-transparan.jpg?s=612x612&w=0&k=20&c=foEv6n4528X0AkgcQZBX6TqWlZAOezpBEgoDRS-5LDo=" alt="Senin-Jumat" class="mx-auto mb-4 h-16 w-16 text-indigo-600">
                <h3 class="text-xl font-semibold text-gray-900">Senin - Jumat</h3>
                <p class="text-lg text-blue-400">09:00 - 18:00</p>
                <p class="mt-2 text-sm text-gray-500">
                  Kami siap melayani Anda pada hari kerja, Senin hingga Jumat, dari pukul 09:00 hingga 18:00. Anda bisa menghubungi kami untuk berbagai kebutuhan, mulai dari konsultasi hingga pemesanan produk.
                </p>
              </div>
            </div>
            
            <!-- Sabtu -->
            <div class="flex justify-center items-center bg-white rounded-xl shadow-md p-6">
              <div class="text-center">
                <img src="https://media.istockphoto.com/id/1780573447/id/vektor/ikon-doodle-kartun-yang-digambar-tangan-tanda-pintu-terbuka-dengan-latar-belakang-putih.jpg?s=612x612&w=0&k=20&c=jn27-Nm3EE_J92m_vuFezE0jVOAIoHIrFErW_5DEi6I=" alt="Sabtu" class="mx-auto mb-4 h-16 w-16 text-indigo-600">
                <h3 class="text-xl font-semibold text-gray-900">Sabtu</h3>
                <p class="text-lg text-blue-400">09:00 - 14:00</p>
                <p class="mt-2 text-sm text-gray-500">
                  Sabtu adalah hari kerja setengah hari, dari pukul 09:00 hingga 14:00. Meskipun waktunya terbatas, kami tetap siap melayani kebutuhan Anda dengan cepat.
                </p>
              </div>
            </div>
            
            <!-- Minggu -->
            <div class="flex justify-center items-center bg-white rounded-xl shadow-md p-6">
              <div class="text-center">
                <img src="https://img.freepik.com/premium-vector/closed-sign-icon-comic-style-accessibility-cartoon-vector-illustration-white-isolated-background-message-splash-effect-business-concept_157943-22063.jpg?ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Minggu" class="mx-auto mb-4 h-16 w-16 text-indigo-600">
                <h3 class="text-xl font-semibold text-gray-900">Minggu</h3>
                <p class="text-lg text-blue-400">Tutup</p>
                <p class="mt-2 text-sm text-gray-500">
                  Minggu adalah hari libur bagi kami. Kami akan kembali melayani Anda pada hari Senin dengan semangat baru!
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- End Jam Kerja -->
      
      <!--features sections-->
      <div class="bg-gray-100 py-24 sm:py-16">
        <div class="mx-auto max-w-7xl px-6 lg:px-16">
          <div class="mx-auto max-w-2xl lg:mx-0 text-center lg:text-left">
            <h2 class="text-4xl font-bold tracking-tight text-gray-900 sm:text-5xl">Layanan Konveksi dari Glam Stitch</h2>
            <p class="mt-6 text-lg text-gray-600">Glam Stitch siap memenuhi kebutuhan produksi pakaian Anda — dari desain custom, manajemen produksi skala besar, hingga kontrol kualitas yang ketat.</p>
          </div>
      
          <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-none">
            <dl class="grid grid-cols-1 gap-x-12 gap-y-16 sm:grid-cols-2 lg:grid-cols-3">
      
              <!-- Desain Custom -->
              <div class="flex flex-col items-center text-center lg:items-start lg:text-left">
                <img src="https://img.freepik.com/premium-photo/female-fashion-designer-cutting-fabric-workbench_1048944-5011017.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Desain Custom Icon" class="w-full max-w-xs h-auto rounded-2xl object-cover shadow-xl mb-6">
                <dt class="text-2xl font-semibold text-gray-900">Desain Pakaian Custom</dt>
                <dd class="mt-3 text-lg text-gray-600">
                  Kami melayani desain pakaian sesuai kebutuhan Anda, baik untuk brand, komunitas, maupun keperluan pribadi.
                  <p class="mt-4">
                    <a href="/#" class="text-base font-semibold text-indigo-600 hover:underline">Selengkapnya <span aria-hidden="true">→</span></a>
                  </p>
                </dd>
              </div>
      
              <!-- Manajemen Produksi -->
              <div class="flex flex-col items-center text-center lg:items-start lg:text-left">
                <img src="https://img.freepik.com/free-photo/portrait-cheerful-good-looking-male-clothes-designer-with-dark-hair-fashionable-outfit-standing-workshop-posing-article-about-his-brand-artist-standing-his-comfy-studio_176420-11848.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Produksi Icon" class="w-full max-w-xs h-auto rounded-2xl object-cover shadow-xl mb-6">
                <dt class="text-2xl font-semibold text-gray-900">Manajemen Produksi</dt>
                <dd class="mt-3 text-lg text-gray-600">
                  Glam Stitch memiliki tim produksi profesional untuk menangani pemesanan dalam jumlah besar secara efisien dan tepat waktu.
                  <p class="mt-4">
                    <a href="/#" class="text-base font-semibold text-indigo-600 hover:underline">Selengkapnya <span aria-hidden="true">→</span></a>
                  </p>
                </dd>
              </div>
      
              <!-- Quality Control -->
              <div class="flex flex-col items-center text-center lg:items-start lg:text-left">
                <img src="https://img.freepik.com/premium-photo/beautiful-young-woman-sewing-clothes-with-sewing-machine_255667-49856.jpg?uid=R108872572&ga=GA1.1.1868222757.1738365469&semt=ais_hybrid&w=740" alt="Quality Check Icon" class="w-full max-w-xs h-auto rounded-2xl object-cover shadow-xl mb-6">
                <dt class="text-2xl font-semibold text-gray-900">Pemeriksaan Kualitas</dt>
                <dd class="mt-3 text-lg text-gray-600">
                  Setiap produk melalui tahapan quality control untuk memastikan kualitas maksimal sebelum dikirimkan kepada Anda.
                  <p class="mt-4">
                    <a href="/#" class="text-base font-semibold text-indigo-600 hover:underline">Selengkapnya <span aria-hidden="true">→</span></a>
                  </p>
                </dd>
              </div>
      
            </dl>
          </div>
        </div>
      </div>
      
      <!--features sections-->
      
      <!--incentives-->
      <div class="bg-white">
        <div class="mx-auto max-w-7xl px-4 py-24 sm:px-6 lg:px-16">
          <div class="rounded-2xl bg-gray-50 px-6 py-16 sm:p-16 border">
            <div class="mx-auto max-w-xl lg:max-w-none">
              <div class="text-center">
                <h2 class="text-2xl font-bold tracking-tight text-gray-900">Konveksi Glam Stitch Mengutamakan Kepuasan Pelanggan</h2>
              </div>
              <div class="mx-auto mt-12 grid max-w-sm grid-cols-1 gap-x-8 gap-y-10 sm:max-w-none lg:grid-cols-3">
                <div class="text-center sm:flex sm:text-left lg:block lg:text-center">
                  <div class="sm:shrink-0">
                    <div class="flow-root">
                      <img class="mx-auto size-16" src="https://tailwindcss.com/plus-assets/img/ecommerce/icons/icon-shipping-simple.svg" alt="">
                    </div>
                  </div>
                  <div class="mt-3 sm:mt-0 sm:ml-6 lg:mt-6 lg:ml-0">
                    <h3 class="text-sm font-medium text-gray-900">Produksi Cepat</h3>
                    <p class="mt-2 text-sm text-gray-500">Konveksi Glam Stitch menawarkan produksi pakaian yang cepat dan tepat waktu untuk memenuhi tenggat waktu Anda tanpa mengurangi kualitas.</p>
                  </div>
                </div>
                <div class="text-center sm:flex sm:text-left lg:block lg:text-center">
                  <div class="sm:shrink-0">
                    <div class="flow-root">
                      <img class="mx-auto size-16" src="https://tailwindcss.com/plus-assets/img/ecommerce/icons/icon-warranty-simple.svg" alt="">
                    </div>
                  </div>
                  <div class="mt-3 sm:mt-0 sm:ml-6 lg:mt-6 lg:ml-0">
                    <h3 class="text-sm font-medium text-gray-900">Jaminan Kualitas</h3>
                    <p class="mt-2 text-sm text-gray-500">Setiap produk dari Konveksi Glam Stitch melalui proses kontrol kualitas yang ketat untuk memastikan kepuasan pelanggan dan daya tahan produk.</p>
                  </div>
                </div>
                <div class="text-center sm:flex sm:text-left lg:block lg:text-center">
                  <div class="sm:shrink-0">
                    <div class="flow-root">
                      <img class="mx-auto size-16" src="https://tailwindcss.com/plus-assets/img/ecommerce/icons/icon-exchange-simple.svg" alt="">
                    </div>
                  </div>
                  <div class="mt-3 sm:mt-0 sm:ml-6 lg:mt-6 lg:ml-0">
                    <h3 class="text-sm font-medium text-gray-900">Pesanan Kustom</h3>
                    <p class="mt-2 text-sm text-gray-500">Konveksi Glam Stitch menerima pesanan pakaian kustom dengan desain, bahan, dan spesifikasi ukuran Anda sendiri.</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      
        
      <!--end incentives-->
      
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
