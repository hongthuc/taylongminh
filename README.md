<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CÔNG TY TNHH MTV TÂY LONG MINH | Thiết Kế & Thi Công Xây Dựng Đà Nẵng</title>
  <meta name="description" content="CÔNG TY TNHH MTV TÂY LONG MINH (taylongminh.com) chuyên thiết kế kiến trúc, thi công phần thô, hoàn thiện, nội thất và xây dựng công trình trọn gói uy tín tại Đà Nẵng. Hotline: 0934.855.348." />

  <!-- Meta thẻ chia sẻ liên kết (Open Graph & Twitter Card dùng logo làm ảnh thumbnail) -->
  <meta property="og:type" content="website" />
  <meta property="og:site_name" content="CÔNG TY TNHH MTV TÂY LONG MINH" />
  <meta property="og:url" content="https://taylongminh.com/" />
  <meta property="og:title" content="CÔNG TY TNHH MTV TÂY LONG MINH - Xây Dựng & Kiến Trúc Đà Nẵng" />
  <meta property="og:description" content="Thiết kế kiến trúc, thi công phần thô, hoàn thiện, nội thất, xây dựng nhà ở và công trình hạ tầng tại Đà Nẵng. Hotline: 0934.855.348." />
  <meta property="og:image" content="https://taylongminh.com/wp-content/uploads/logo-tay-long-minh.png" />
  <meta property="og:image:alt" content="Logo CÔNG TY TNHH MTV TÂY LONG MINH" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="CÔNG TY TNHH MTV TÂY LONG MINH | taylongminh.com" />
  <meta name="twitter:description" content="Đơn vị thi công xây dựng uy tín tại Hòa Vang - TP Đà Nẵng. Hotline: 0934.855.348." />
  <meta name="twitter:image" content="https://taylongminh.com/wp-content/uploads/logo-tay-long-minh.png" />

  <!-- Favicon Logo Tây Long Minh -->
  <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='12' fill='%230F2B4C'/%3E%3Cpath d='M14 48V24L32 12L50 24V48H41V29L32 23L23 29V48H14Z' fill='%23C88A2E'/%3E%3Crect x='28' y='34' width='8' height='14' fill='%23FFFFFF'/%3E%3C/svg%3E" />

  <!-- Google Fonts: Inter -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" />

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
          },
          colors: {
            brand: {
              navy: '#0F2B4C',
              navyDark: '#0A1E36',
              navyLight: '#1B3F6B',
              gold: '#C88A2E',
              goldDark: '#A66F1D',
              goldLight: '#FBF5EA',
            }
          }
        }
      }
    };
  </script>

  <style>
    /* Đảm bảo tuyệt đối không tràn viền ngang và không lệch sang phải trên mọi thiết bị */
    *, *::before, *::after {
      box-sizing: border-box;
    }
    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      max-width: 100%;
      overflow-x: hidden;
      scroll-behavior: smooth;
      font-family: 'Inter', sans-serif;
      color: #1E293B;
      background-color: #FFFFFF;
    }

    /* Chiều ngang chuẩn 95% màn hình trên máy tính (>=1024px) và full gọn trên điện thoại */
    .tlm-container {
      width: 100%;
      margin-left: auto;
      margin-right: auto;
      padding-left: 12px;
      padding-right: 12px;
    }
    @media (min-width: 640px) {
      .tlm-container {
        padding-left: 18px;
        padding-right: 18px;
      }
    }
    @media (min-width: 1024px) {
      .tlm-container {
        width: 95%;
        max-width: 95%;
        padding-left: 0;
        padding-right: 0;
      }
    }

    /* Flatsome Dropdown Menu gọn gàng */
    .nav-item-dropdown:hover .nav-dropdown-panel {
      opacity: 1;
      visibility: visible;
      transform: translateY(0);
    }
    .nav-dropdown-panel {
      opacity: 0;
      visibility: hidden;
      transform: translateY(6px);
      transition: all 0.2s ease;
    }

    /* Hero Slider: 2 banner kích thước bằng nhau tuyệt đối, chữ luôn nằm trọn bên trong */
    .hero-slider-grid {
      display: grid;
      grid-template-columns: 1fr;
      grid-template-rows: 1fr;
      position: relative;
      width: 100%;
      overflow: hidden;
    }
    .hero-slide {
      grid-area: 1 / 1;
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.65s ease-in-out, visibility 0.65s ease-in-out;
      width: 100%;
      height: 100%;
    }
    .hero-slide.active {
      opacity: 1;
      visibility: visible;
      z-index: 2;
    }

    /* Thanh danh mục không xuống dòng tên từng danh mục */
    .cat-no-wrap {
      white-space: nowrap;
      flex-shrink: 0;
    }

    /* Ẩn thanh cuộn ngang nhưng vẫn vuốt mượt trên điện thoại */
    .no-scrollbar::-webkit-scrollbar {
      display: none;
    }
    .no-scrollbar {
      -ms-overflow-style: none;
      scrollbar-width: none;
    }

    /* Hiệu ứng nhẹ cho nút liên hệ nổi */
    @keyframes subtlePulse {
      0% { box-shadow: 0 0 0 0 rgba(200, 138, 46, 0.45); }
      70% { box-shadow: 0 0 0 10px rgba(200, 138, 46, 0); }
      100% { box-shadow: 0 0 0 0 rgba(200, 138, 46, 0); }
    }
    .pulse-ring {
      animation: subtlePulse 2.2s infinite;
    }

    /* Đường gạch chân tiêu đề phong cách Flatsome */
    .flatsome-divider {
      width: 56px;
      height: 3px;
      background-color: #C88A2E;
      border-radius: 999px;
    }
  </style>
</head>
<body class="bg-white text-slate-800 antialiased">

  <!-- ==================== 1. TOP BAR (FLATSOME STYLE) ==================== -->
  <div class="bg-brand-navy text-white text-xs border-b border-brand-navyLight">
    <div class="tlm-container py-2 flex flex-wrap items-center justify-between gap-2">
      <div class="flex items-center gap-3 sm:gap-5 flex-wrap">
        <a href="tel:0934855348" class="inline-flex items-center gap-1.5 hover:text-brand-gold transition-colors">
          <i class="fa-solid fa-phone text-brand-gold text-[11px]"></i>
          <span class="font-medium">0934.855.348</span>
        </a>
        <span class="hidden sm:inline text-white/30">|</span>
        <span class="hidden sm:inline-flex items-center gap-1.5 text-slate-200">
          <i class="fa-solid fa-location-dot text-brand-gold text-[11px]"></i>
          <span>Thôn Cẩm Toại Tây, Xã Hòa Vang, TP Đà Nẵng</span>
        </span>
      </div>
      <div class="flex items-center gap-3 text-slate-200">
        <span class="hidden md:inline text-[11px] tracking-wide">taylongminh.com</span>
        <a href="#fanpage-section" aria-label="Facebook Tây Long Minh" class="hover:text-brand-gold transition-colors">
          <i class="fa-brands fa-facebook-f"></i>
        </a>
        <a href="https://zalo.me/0934855348" target="_blank" rel="noopener" aria-label="Zalo Tây Long Minh" class="hover:text-brand-gold transition-colors font-bold text-[11px]">
          Zalo
        </a>
      </div>
    </div>
  </div>

  <!-- ==================== 2. HEADER & NAVIGATION (KHÔNG NÚT GỌI NGAY ĐỂ TRÁNH TRÀN VIỀN) ==================== -->
  <header class="sticky top-0 z-40 bg-white/95 backdrop-blur-md border-b border-slate-200 shadow-sm w-full">
    <div class="tlm-container h-16 sm:h-[70px] flex items-center justify-between gap-3">
      
      <!-- Logo Công Ty TNHH MTV Tây Long Minh (Thiết kế chuyên nghiệp, gọn nhỏ tinh tế) -->
      <a href="#trang-chu" class="flex items-center gap-2.5 shrink-0 group focus:outline-none" aria-label="Trang chủ Công Ty TNHH MTV Tây Long Minh">
        <svg class="w-9 h-9 sm:w-10 sm:h-10 shrink-0" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Logo Tây Long Minh">
          <rect width="64" height="64" rx="12" fill="#0F2B4C"/>
          <!-- Khung kiến trúc hình học -->
          <path d="M12 48V24.5L32 11L52 24.5V48H43.5V29L32 21.2L20.5 29V48H12Z" fill="#C88A2E"/>
          <!-- Cột trụ trung tâm chữ T cách điệu -->
          <path d="M25.5 31H38.5V35.5H34.25V48H29.75V35.5H25.5V31Z" fill="#FFFFFF"/>
          <!-- Đường nền móng vững chắc -->
          <rect x="12" y="51" width="40" height="3.2" rx="1.6" fill="#FFFFFF" fill-opacity="0.9"/>
        </svg>
        <div class="flex flex-col leading-tight">
          <span class="text-[14px] sm:text-[15.5px] font-extrabold tracking-tight text-brand-navy group-hover:text-brand-gold transition-colors whitespace-nowrap">
            TÂY LONG MINH
          </span>
          <span class="text-[9.5px] sm:text-[10px] font-semibold tracking-wider text-brand-gold uppercase whitespace-nowrap">
            Xây Dựng &amp; Kiến Trúc
          </span>
        </div>
      </a>

      <!-- Menu Chính Desktop: Viết liền trên 1 hàng, chữ nhỏ gọn, tuyệt đối không xuống dòng -->
      <nav class="hidden lg:flex items-center justify-end flex-nowrap gap-3.5 xl:gap-5" aria-label="Điều hướng chính">
        <a href="#trang-chu" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-brand-navy hover:text-brand-gold transition-colors py-2">
          Trang chủ
        </a>
        <a href="#gioi-thieu" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-slate-700 hover:text-brand-gold transition-colors py-2">
          Giới thiệu
        </a>

        <!-- Dropdown Công trình thực tế -->
        <div class="relative nav-item-dropdown py-2">
          <a href="#du-an-da-nang" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-slate-700 hover:text-brand-gold transition-colors inline-flex items-center gap-1">
            Công trình thực tế
            <i class="fa-solid fa-chevron-down text-[9px] text-slate-400"></i>
          </a>
          <div class="nav-dropdown-panel absolute left-0 top-full w-56 bg-white rounded-lg shadow-lg border border-slate-100 py-2 z-50">
            <a href="#du-an-da-nang" onclick="filterProjects('khach-san')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Khách sạn – Căn hộ – Phòng trọ</a>
            <a href="#du-an-da-nang" onclick="filterProjects('biet-thu')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Biệt thự</a>
            <a href="#du-an-da-nang" onclick="filterProjects('nha-pho')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Nhà phố</a>
            <a href="#du-an-da-nang" onclick="filterProjects('van-phong')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Văn phòng &amp; Hạ tầng</a>
          </div>
        </div>

        <!-- Dropdown Lĩnh vực hoạt động -->
        <div class="relative nav-item-dropdown py-2">
          <a href="#san-pham-thi-cong" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-slate-700 hover:text-brand-gold transition-colors inline-flex items-center gap-1">
            Lĩnh vực hoạt động
            <i class="fa-solid fa-chevron-down text-[9px] text-slate-400"></i>
          </a>
          <div class="nav-dropdown-panel absolute left-0 top-full w-56 bg-white rounded-lg shadow-lg border border-slate-100 py-2 z-50">
            <a href="#san-pham-thi-cong" onclick="filterProducts('thiet-ke')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Thiết kế Kiến trúc – Nội thất</a>
            <a href="#san-pham-thi-cong" onclick="filterProducts('phan-tho')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Thi công phần thô</a>
            <a href="#san-pham-thi-cong" onclick="filterProducts('hoan-thien')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Thi công hoàn thiện</a>
            <a href="#san-pham-thi-cong" onclick="filterProducts('ha-tang')" class="block px-4 py-2 text-xs font-medium text-slate-700 hover:bg-brand-goldLight hover:text-brand-navy">Xây dựng hạ tầng &amp; Cải tạo</a>
          </div>
        </div>

        <a href="#san-pham-thi-cong" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-slate-700 hover:text-brand-gold transition-colors py-2">
          Mẫu thiết kế
        </a>
        <a href="#bao-gia" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-slate-700 hover:text-brand-gold transition-colors py-2">
          Báo giá
        </a>
        <a href="#tin-tuc" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-slate-700 hover:text-brand-gold transition-colors py-2">
          Tin tức
        </a>
        <a href="#lien-he" class="cat-no-wrap text-[12.5px] xl:text-[13.5px] font-semibold text-slate-700 hover:text-brand-gold transition-colors py-2">
          Liên hệ
        </a>
      </nav>

      <!-- Nút mở Menu Mobile -->
      <button id="mobileMenuBtn" type="button" aria-label="Mở menu điều hướng" class="lg:hidden inline-flex items-center justify-center w-10 h-10 rounded-lg border border-slate-200 text-brand-navy hover:bg-slate-50 transition-colors shrink-0">
        <i class="fa-solid fa-bars text-lg"></i>
      </button>
    </div>

    <!-- Menu Mobile Drawer -->
    <div id="mobileMenuPanel" class="hidden lg:hidden bg-white border-t border-slate-200 shadow-lg w-full">
      <div class="tlm-container py-3 flex flex-col divide-y divide-slate-100">
        <a href="#trang-chu" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-brand-navy">Trang chủ</a>
        <a href="#gioi-thieu" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-slate-700">Giới thiệu</a>
        <a href="#san-pham-thi-cong" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-slate-700">Lĩnh vực &amp; Sản phẩm thi công</a>
        <a href="#du-an-da-nang" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-slate-700">Dự án tại Đà Nẵng</a>
        <a href="#bao-gia" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-slate-700">Yêu cầu &amp; Báo giá</a>
        <a href="#tin-tuc" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-slate-700">Tin tức xây dựng</a>
        <a href="#doi-tac" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-slate-700">Đối tác tiêu biểu</a>
        <a href="#lien-he" onclick="closeMobileMenu()" class="py-2.5 text-sm font-semibold text-slate-700">Bản đồ &amp; Liên hệ</a>
      </div>
    </div>
  </header>

  <!-- ==================== 3. HERO BANNER TỰ TRƯỢT (2 BANNER KÍCH THƯỚC BẰNG NHAU, CHỮ NẰM GỌN TRONG BANNER) ==================== -->
  <section id="trang-chu" class="w-full bg-slate-100 py-3 sm:py-4">
    <div class="tlm-container">
      <div class="relative rounded-xl overflow-hidden shadow-md bg-brand-navy" id="heroSliderContainer">
        <div class="hero-slider-grid">

          <!-- BANNER 1 -->
          <div class="hero-slide active relative flex items-center">
            <!-- Ảnh nền công trình thực tế -->
            <img
              data-drive-id="13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz"
              src="https://lh3.googleusercontent.com/d/13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz=w1400"
              alt="Thi công xây dựng trọn gói Công Ty TNHH MTV Tây Long Minh"
              class="absolute inset-0 w-full h-full object-cover object-center"
            />
            <!-- Lớp phủ chuyển sắc chuẩn màu logo giúp chữ luôn sắc nét -->
            <div class="absolute inset-0 bg-gradient-to-r from-brand-navyDark/95 via-brand-navy/85 to-brand-navy/55"></div>

            <!-- Nội dung nằm trọn trong khung với lề an toàn cách xa 4 viền banner -->
            <div class="relative z-10 w-full px-12 sm:px-16 md:px-20 lg:px-24 py-10 sm:py-14 md:py-16 lg:py-20">
              <div class="max-w-2xl">
                <p class="text-[11px] sm:text-xs md:text-sm font-bold tracking-widest uppercase text-brand-gold mb-2 sm:mb-3">
                  CÔNG TY TNHH MTV TÂY LONG MINH
                </p>
                <h1 class="text-xl sm:text-3xl md:text-4xl lg:text-[42px] font-extrabold text-white leading-snug mb-3 sm:mb-4">
                  Thiết Kế &amp; Thi Công Xây Dựng Trọn Gói Chuyên Nghiệp Tại Đà Nẵng
                </h1>
                <p class="text-xs sm:text-sm md:text-base text-slate-200 leading-relaxed mb-5 sm:mb-6">
                  An toàn – Chất lượng – Đúng tiến độ cho mọi công trình nhà phố, biệt thự, căn hộ, khách sạn và hạ tầng dân dụng khu vực Đà Nẵng – Miền Trung.
                </p>
                <div class="flex flex-wrap items-center gap-2.5 sm:gap-3">
                  <a href="#bao-gia" class="inline-flex items-center justify-center px-4 sm:px-6 py-2.5 sm:py-3 rounded-lg bg-brand-gold hover:bg-brand-goldDark text-white font-semibold text-xs sm:text-sm transition-colors shadow">
                    Nhận báo giá miễn phí
                  </a>
                  <a href="#du-an-da-nang" class="inline-flex items-center justify-center px-4 sm:px-6 py-2.5 sm:py-3 rounded-lg bg-white/15 hover:bg-white/25 text-white border border-white/30 font-semibold text-xs sm:text-sm transition-colors">
                    Xem dự án thực tế
                  </a>
                </div>
              </div>
            </div>
          </div>

          <!-- BANNER 2 (Cấu trúc & khoảng đệm đồng nhất 100% với Banner 1 để 2 ảnh bằng kích thước nhau) -->
          <div class="hero-slide relative flex items-center">
            <img
              data-drive-id="157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT"
              src="https://lh3.googleusercontent.com/d/157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT=w1400"
              alt="Dự án thực tế tại Đà Nẵng - Tây Long Minh"
              class="absolute inset-0 w-full h-full object-cover object-center"
            />
            <div class="absolute inset-0 bg-gradient-to-r from-brand-navyDark/95 via-brand-navy/85 to-brand-navy/55"></div>

            <div class="relative z-10 w-full px-12 sm:px-16 md:px-20 lg:px-24 py-10 sm:py-14 md:py-16 lg:py-20">
              <div class="max-w-2xl">
                <p class="text-[11px] sm:text-xs md:text-sm font-bold tracking-widest uppercase text-brand-gold mb-2 sm:mb-3">
                  NHÀ Ở GIA ĐÌNH – TIÊU CHUẨN CÔNG TRÌNH
                </p>
                <h2 class="text-xl sm:text-3xl md:text-4xl lg:text-[42px] font-extrabold text-white leading-snug mb-3 sm:mb-4">
                  Giải Pháp Xây Dựng Bền Vững, Tối Ưu Chi Phí &amp; Minh Bạch Vật Tư
                </h2>
                <p class="text-xs sm:text-sm md:text-base text-slate-200 leading-relaxed mb-5 sm:mb-6">
                  Đội ngũ kỹ sư và thợ lành nghề trực tiếp giám sát thi công phần thô, hoàn thiện nội ngoại thất và bảo hành công trình lâu dài.
                </p>
                <div class="flex flex-wrap items-center gap-2.5 sm:gap-3">
                  <a href="#san-pham-thi-cong" class="inline-flex items-center justify-center px-4 sm:px-6 py-2.5 sm:py-3 rounded-lg bg-brand-gold hover:bg-brand-goldDark text-white font-semibold text-xs sm:text-sm transition-colors shadow">
                    Xem danh mục thi công
                  </a>
                  <a href="tel:0934855348" class="inline-flex items-center justify-center px-4 sm:px-6 py-2.5 sm:py-3 rounded-lg bg-white/15 hover:bg-white/25 text-white border border-white/30 font-semibold text-xs sm:text-sm transition-colors">
                    Hotline: 0934.855.348
                  </a>
                </div>
              </div>
            </div>
          </div>

        </div>

        <!-- Nút chuyển slide trái / phải đặt sát mép ngoài, tách biệt hoàn toàn với vùng chữ -->
        <button type="button" id="prevSlideBtn" aria-label="Banner trước" class="absolute left-2 sm:left-3.5 top-1/2 -translate-y-1/2 z-20 w-8 h-8 sm:w-10 sm:h-10 rounded-full bg-black/35 hover:bg-brand-gold text-white flex items-center justify-center transition-colors">
          <i class="fa-solid fa-chevron-left text-xs sm:text-sm"></i>
        </button>
        <button type="button" id="nextSlideBtn" aria-label="Banner kế tiếp" class="absolute right-2 sm:right-3.5 top-1/2 -translate-y-1/2 z-20 w-8 h-8 sm:w-10 sm:h-10 rounded-full bg-black/35 hover:bg-brand-gold text-white flex items-center justify-center transition-colors">
          <i class="fa-solid fa-chevron-right text-xs sm:text-sm"></i>
        </button>

        <!-- Chấm chỉ báo slide đặt dưới đáy -->
        <div class="absolute bottom-3 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
          <button type="button" onclick="goToSlide(0)" class="hero-dot w-6 h-2 rounded-full bg-brand-gold transition-all" aria-label="Xem banner 1"></button>
          <button type="button" onclick="goToSlide(1)" class="hero-dot w-2.5 h-2 rounded-full bg-white/50 hover:bg-white transition-all" aria-label="Xem banner 2"></button>
        </div>
      </div>
    </div>
  </section>

  <!-- ==================== 4. DANH MỤC NHANH TRANG CHỦ (CHỮ NHỎ GỌN, 1 HÀNG TRÊN MÁY TÍNH, KHÔNG XUỐNG DÒNG TÊN DANH MỤC) ==================== -->
  <section class="w-full bg-white border-b border-slate-200 py-3.5">
    <div class="tlm-container">
      <div class="flex items-center lg:justify-center gap-2 overflow-x-auto lg:overflow-visible lg:flex-wrap no-scrollbar py-0.5">
        <a href="#san-pham-thi-cong" onclick="filterProducts('all')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-brand-navy text-white text-[12px] font-semibold hover:bg-brand-gold transition-colors">
          Tất cả hạng mục
        </a>
        <a href="#san-pham-thi-cong" onclick="filterProducts('thiet-ke')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Thiết kế Kiến trúc – Nội thất
        </a>
        <a href="#san-pham-thi-cong" onclick="filterProducts('phan-tho')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Thi công phần thô
        </a>
        <a href="#san-pham-thi-cong" onclick="filterProducts('hoan-thien')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Thi công hoàn thiện
        </a>
        <a href="#san-pham-thi-cong" onclick="filterProducts('ha-tang')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Hạ tầng &amp; Thủy lợi
        </a>
        <a href="#du-an-da-nang" onclick="filterProjects('khach-san')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Khách sạn – Căn hộ
        </a>
        <a href="#du-an-da-nang" onclick="filterProjects('biet-thu')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Biệt thự
        </a>
        <a href="#du-an-da-nang" onclick="filterProjects('nha-pho')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Nhà phố
        </a>
        <a href="#du-an-da-nang" onclick="filterProjects('van-phong')" class="cat-no-wrap px-3 py-1.5 rounded-lg bg-slate-100 text-slate-700 text-[12px] font-semibold hover:bg-brand-goldLight hover:text-brand-navy transition-colors">
          Văn phòng
        </a>
      </div>
    </div>
  </section>

  <!-- ==================== 5. DỊCH VỤ TIÊU BIỂU (UX BUILDER 3 COLUMNS - GIỐNG WEB MẪU) ==================== -->
  <section class="py-10 sm:py-12 bg-slate-50">
    <div class="tlm-container">
      <div class="text-center mb-8">
        <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-tight">Dịch Vụ Tiêu Biểu</h2>
        <div class="flatsome-divider mx-auto mt-2.5"></div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-4 sm:gap-6">
        <!-- Cột 1: Thiết kế -->
        <a href="#san-pham-thi-cong" onclick="filterProducts('thiet-ke')" class="group bg-white rounded-xl p-6 border border-slate-200 hover:border-brand-gold shadow-sm hover:shadow-md transition-all text-center flex flex-col items-center">
          <div class="w-14 h-14 rounded-xl bg-brand-navy text-brand-gold flex items-center justify-center mb-4 group-hover:bg-brand-gold group-hover:text-white transition-colors">
            <i class="fa-solid fa-compass-drafting text-2xl"></i>
          </div>
          <h3 class="text-base sm:text-lg font-bold text-brand-navy uppercase mb-2">Thiết Kế Kiến Trúc</h3>
          <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
            Thiết kế nhà phố, biệt thự, khách sạn, căn hộ và không gian làm việc tối ưu công năng, thẩm mỹ hiện đại và phong thủy hài hòa.
          </p>
        </a>

        <!-- Cột 2: Thi công -->
        <a href="#san-pham-thi-cong" onclick="filterProducts('phan-tho')" class="group bg-white rounded-xl p-6 border border-slate-200 hover:border-brand-gold shadow-sm hover:shadow-md transition-all text-center flex flex-col items-center">
          <div class="w-14 h-14 rounded-xl bg-brand-navy text-brand-gold flex items-center justify-center mb-4 group-hover:bg-brand-gold group-hover:text-white transition-colors">
            <i class="fa-solid fa-helmet-safety text-2xl"></i>
          </div>
          <h3 class="text-base sm:text-lg font-bold text-brand-navy uppercase mb-2">Thi Công Xây Dựng</h3>
          <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
            Thi công phần thô, xây nhà trọn gói, công trình dân dụng, san lấp mặt bằng và duy tu hạ tầng thủy lợi chuẩn kỹ thuật tại Đà Nẵng.
          </p>
        </a>

        <!-- Cột 3: Nội thất & Hoàn thiện -->
        <a href="#san-pham-thi-cong" onclick="filterProducts('hoan-thien')" class="group bg-white rounded-xl p-6 border border-slate-200 hover:border-brand-gold shadow-sm hover:shadow-md transition-all text-center flex flex-col items-center">
          <div class="w-14 h-14 rounded-xl bg-brand-navy text-brand-gold flex items-center justify-center mb-4 group-hover:bg-brand-gold group-hover:text-white transition-colors">
            <i class="fa-solid fa-couch text-2xl"></i>
          </div>
          <h3 class="text-base sm:text-lg font-bold text-brand-navy uppercase mb-2">Hoàn Thiện &amp; Nội Thất</h3>
          <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
            Hoàn thiện công trình, lắp đặt hệ thống điện nước đồng bộ và thi công nội thất sắc nét theo đúng bản vẽ và ngân sách đầu tư.
          </p>
        </a>
      </div>
    </div>
  </section>

  <!-- ==================== 6. GIỚI THIỆU & THẾ MẠNH CỦA CHÚNG TÔI (MÔ PHỎNG BỐ CỤC FLATSOME TÍN TRƯỜNG THỊNH) ==================== -->
  <section id="gioi-thieu" class="py-10 sm:py-14 bg-white">
    <div class="tlm-container">
      <!-- Giới thiệu Công ty -->
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 sm:gap-8 items-center mb-12">
        <div class="lg:col-span-5">
          <div class="rounded-xl overflow-hidden shadow-md border border-slate-200 aspect-[4/3] bg-slate-100">
            <img
              data-drive-id="1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR"
              src="https://lh3.googleusercontent.com/d/1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR=w1000"
              alt="Đội ngũ thi công thực tế Công Ty TNHH MTV Tây Long Minh"
              class="w-full h-full object-cover"
            />
          </div>
        </div>
        <div class="lg:col-span-7">
          <p class="text-xs font-bold uppercase tracking-widest text-brand-gold mb-1.5">Về chúng tôi</p>
          <h2 class="text-xl sm:text-2xl lg:text-3xl font-extrabold text-brand-navy mb-3">
            CÔNG TY TNHH MTV TÂY LONG MINH
          </h2>
          <div class="flatsome-divider mb-4"></div>
          <p class="text-sm sm:text-[15px] text-slate-600 leading-relaxed mb-3">
            <strong>CÔNG TY TNHH MTV TÂY LONG MINH</strong> (Mã số thuế: <strong>0402185216</strong>) có trụ sở tại Thôn Cẩm Toại Tây, Xã Hòa Vang, TP Đà Nẵng. Chúng tôi chuyên sâu trong lĩnh vực <strong>Thiết kế – Thi công xây dựng nhà ở dân dụng, nhà phố, biệt thự, khách sạn, căn hộ, hoàn thiện nội ngoại thất và công trình hạ tầng kỹ thuật – thủy lợi</strong> tại Đà Nẵng và khu vực lân cận.
          </p>
          <p class="text-sm sm:text-[15px] text-slate-600 leading-relaxed mb-5">
            Với phương châm đặt chữ <strong>“TÂM”</strong> và <strong>“TÍN”</strong> lên hàng đầu, mỗi công trình Tây Long Minh thực hiện đều đảm bảo 4 tiêu chuẩn cốt lõi: <strong>An Toàn – Chất Lượng – Đúng Tiến Độ – Chi Phí Minh Bạch</strong>.
          </p>
          <div class="grid grid-cols-3 gap-3 sm:gap-4 pt-3 border-t border-slate-200">
            <div>
              <div class="text-xl sm:text-2xl font-extrabold text-brand-navy">100%</div>
              <div class="text-[11px] sm:text-xs text-slate-500 mt-0.5">Đúng tiến độ cam kết</div>
            </div>
            <div>
              <div class="text-xl sm:text-2xl font-extrabold text-brand-gold">24/7</div>
              <div class="text-[11px] sm:text-xs text-slate-500 mt-0.5">Tư vấn &amp; khảo sát</div>
            </div>
            <div>
              <div class="text-xl sm:text-2xl font-extrabold text-brand-navy">5 Năm</div>
              <div class="text-[11px] sm:text-xs text-slate-500 mt-0.5">Bảo hành kết cấu</div>
            </div>
          </div>
        </div>
      </div>

      <!-- 6 Thế mạnh của chúng tôi -->
      <div class="pt-4">
        <div class="text-center mb-8">
          <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-tight">Thế Mạnh Của Chúng Tôi</h2>
          <div class="flatsome-divider mx-auto mt-2.5"></div>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4 sm:gap-5">
          <div class="bg-slate-50 rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
            <div class="w-10 h-10 rounded-lg bg-brand-navy text-brand-gold flex items-center justify-center shrink-0">
              <i class="fa-solid fa-users-gear text-base"></i>
            </div>
            <div>
              <h3 class="text-sm sm:text-[15px] font-bold text-brand-navy mb-1">Đội ngũ kỹ sư, thợ lành nghề</h3>
              <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">Kỹ sư giàu kinh nghiệm hiện trường cùng tổ đội thi công trực tiếp tay nghề cao, tận tâm với từng chi tiết.</p>
            </div>
          </div>

          <div class="bg-slate-50 rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
            <div class="w-10 h-10 rounded-lg bg-brand-navy text-brand-gold flex items-center justify-center shrink-0">
              <i class="fa-solid fa-layer-group text-base"></i>
            </div>
            <div>
              <h3 class="text-sm sm:text-[15px] font-bold text-brand-navy mb-1">Vật liệu &amp; kỹ thuật hiện đại</h3>
              <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">Cập nhật xu hướng thiết kế mới, sử dụng vật tư chính hãng đúng chủng loại hợp đồng, minh bạch xuất xứ.</p>
            </div>
          </div>

          <div class="bg-slate-50 rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
            <div class="w-10 h-10 rounded-lg bg-brand-navy text-brand-gold flex items-center justify-center shrink-0">
              <i class="fa-solid fa-clipboard-check text-base"></i>
            </div>
            <div>
              <h3 class="text-sm sm:text-[15px] font-bold text-brand-navy mb-1">Giám sát tiến độ chuẩn xác</h3>
              <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">Cập nhật nhật ký thi công hằng ngày giúp chủ đầu tư dễ dàng theo dõi tiến độ và chất lượng từ xa.</p>
            </div>
          </div>

          <div class="bg-slate-50 rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
            <div class="w-10 h-10 rounded-lg bg-brand-navy text-brand-gold flex items-center justify-center shrink-0">
              <i class="fa-solid fa-shield-halved text-base"></i>
            </div>
            <div>
              <h3 class="text-sm sm:text-[15px] font-bold text-brand-navy mb-1">Bảo hành công trình lâu dài</h3>
              <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">Chính sách hậu mãi chu đáo, hỗ trợ kỹ thuật nhanh chóng ngay khi khách hàng cần bảo trì công trình.</p>
            </div>
          </div>

          <div class="bg-slate-50 rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
            <div class="w-10 h-10 rounded-lg bg-brand-navy text-brand-gold flex items-center justify-center shrink-0">
              <i class="fa-solid fa-file-invoice-dollar text-base"></i>
            </div>
            <div>
              <h3 class="text-sm sm:text-[15px] font-bold text-brand-navy mb-1">Chi phí tối ưu, không phát sinh</h3>
              <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">Bóc tách dự toán chi tiết từng hạng mục ngay từ đầu, cân đối ngân sách hợp lý nhất cho chủ đầu tư.</p>
            </div>
          </div>

          <div class="bg-slate-50 rounded-xl p-5 border border-slate-200 flex items-start gap-3.5">
            <div class="w-10 h-10 rounded-lg bg-brand-navy text-brand-gold flex items-center justify-center shrink-0">
              <i class="fa-solid fa-headset text-base"></i>
            </div>
            <div>
              <h3 class="text-sm sm:text-[15px] font-bold text-brand-navy mb-1">Hỗ trợ tư vấn miễn phí 24/7</h3>
              <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">Sẵn sàng khảo sát thực tế tận nơi tại Đà Nẵng, tư vấn phương án thi công và hồ sơ pháp lý hoàn toàn miễn phí.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ==================== 7. SẢN PHẨM & HẠNG MỤC THI CÔNG THỰC TẾ (9 ẢNH DRIVE, 2 CỘT MOBILE, KHÔNG NHÃN DÁN, KHÔNG CẮT CHỮ) ==================== -->
  <section id="san-pham-thi-cong" class="py-10 sm:py-14 bg-slate-50 border-t border-slate-200">
    <div class="tlm-container">
      <div class="text-center mb-6">
        <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-tight">
          Danh Mục Sản Phẩm &amp; Thi Công Thực Tế
        </h2>
        <div class="flatsome-divider mx-auto mt-2.5"></div>
      </div>

      <!-- Bộ lọc danh mục sản phẩm (Viết liền trên 1 hàng ở máy tính, chữ nhỏ gọn) -->
      <div class="flex items-center lg:justify-center gap-2 overflow-x-auto lg:overflow-visible lg:flex-wrap no-scrollbar mb-7 pb-1" id="productFilterTabs">
        <button type="button" data-cat="all" onclick="filterProducts('all')" class="product-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-brand-navy text-white transition-colors">
          Tất cả
        </button>
        <button type="button" data-cat="thiet-ke" onclick="filterProducts('thiet-ke')" class="product-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-white text-slate-700 border border-slate-200 hover:border-brand-gold transition-colors">
          Thiết kế Kiến trúc – Nội thất
        </button>
        <button type="button" data-cat="phan-tho" onclick="filterProducts('phan-tho')" class="product-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-white text-slate-700 border border-slate-200 hover:border-brand-gold transition-colors">
          Thi công phần thô
        </button>
        <button type="button" data-cat="hoan-thien" onclick="filterProducts('hoan-thien')" class="product-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-white text-slate-700 border border-slate-200 hover:border-brand-gold transition-colors">
          Thi công hoàn thiện
        </button>
        <button type="button" data-cat="ha-tang" onclick="filterProducts('ha-tang')" class="product-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-white text-slate-700 border border-slate-200 hover:border-brand-gold transition-colors">
          Hạ tầng &amp; Cải tạo
        </button>
      </div>

      <!-- Lưới sản phẩm: 2 cột trên điện thoại, 3 cột cân đối trên máy tính; sạch đẹp không nhãn dán -->
      <div id="productsGrid" class="grid grid-cols-2 md:grid-cols-3 gap-3 sm:gap-5"></div>
    </div>
  </section>

  <!-- ==================== 8. DỰ ÁN TIÊU BIỂU TẠI ĐÀ NẴNG (10 ẢNH DRIVE, 2 CỘT MOBILE, 5 CỘT DESKTOP) ==================== -->
  <section id="du-an-da-nang" class="py-10 sm:py-14 bg-white border-t border-slate-200">
    <div class="tlm-container">
      <div class="text-center mb-6">
        <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-tight">
          Các Dự Án Tiêu Biểu Tại Đà Nẵng
        </h2>
        <div class="flatsome-divider mx-auto mt-2.5"></div>
      </div>

      <!-- Bộ lọc danh mục dự án giống web mẫu (Viết gọn không xuống dòng tên danh mục) -->
      <div class="flex items-center lg:justify-center gap-2 overflow-x-auto lg:overflow-visible lg:flex-wrap no-scrollbar mb-7 pb-1" id="projectFilterTabs">
        <button type="button" data-cat="all" onclick="filterProjects('all')" class="project-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-brand-navy text-white transition-colors">
          Tất cả
        </button>
        <button type="button" data-cat="khach-san" onclick="filterProjects('khach-san')" class="project-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-slate-100 text-slate-700 hover:bg-brand-goldLight transition-colors">
          Khách sạn – Căn hộ – Phòng trọ
        </button>
        <button type="button" data-cat="biet-thu" onclick="filterProjects('biet-thu')" class="project-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-slate-100 text-slate-700 hover:bg-brand-goldLight transition-colors">
          Biệt thự
        </button>
        <button type="button" data-cat="nha-pho" onclick="filterProjects('nha-pho')" class="project-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-slate-100 text-slate-700 hover:bg-brand-goldLight transition-colors">
          Nhà phố
        </button>
        <button type="button" data-cat="van-phong" onclick="filterProjects('van-phong')" class="project-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-slate-100 text-slate-700 hover:bg-brand-goldLight transition-colors">
          Văn phòng &amp; Hạ tầng
        </button>
      </div>

      <!-- Lưới 10 dự án Đà Nẵng: 2 cột trên điện thoại, 5 cột trên máy tính (2 hàng tròn trịa) -->
      <div id="projectsGrid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-3 sm:gap-4"></div>
    </div>
  </section>

  <!-- ==================== 9. FORM YÊU CẦU TƯ VẤN & BÁO GIÁ MIỄN PHÍ TRANG CHỦ ==================== -->
  <section id="bao-gia" class="py-10 sm:py-14 bg-brand-navy text-white">
    <div class="tlm-container">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
        <!-- Thông tin hướng dẫn báo giá -->
        <div class="lg:col-span-5">
          <p class="text-xs font-bold uppercase tracking-widest text-brand-gold mb-2">Miễn phí tư vấn &amp; khảo sát</p>
          <h2 class="text-2xl sm:text-3xl font-extrabold leading-tight mb-4">
            Đăng Ký Nhận Báo Giá Thi Công Chi Tiết
          </h2>
          <div class="flatsome-divider mb-5"></div>
          <p class="text-sm text-slate-300 leading-relaxed mb-6">
            Để lại thông tin công trình của quý khách, kỹ sư của <strong>CÔNG TY TNHH MTV TÂY LONG MINH</strong> sẽ liên hệ tư vấn phương án kỹ thuật và gửi bảng dự toán chi tiết trong thời gian sớm nhất.
          </p>
          <div class="space-y-3 text-sm">
            <div class="flex items-center gap-3">
              <div class="w-9 h-9 rounded-lg bg-white/10 text-brand-gold flex items-center justify-center shrink-0">
                <i class="fa-solid fa-phone-volume"></i>
              </div>
              <div>
                <div class="text-xs text-slate-400">Hotline tư vấn trực tiếp</div>
                <a href="tel:0934855348" class="font-bold text-white hover:text-brand-gold">0934.855.348</a>
              </div>
            </div>
            <div class="flex items-center gap-3">
              <div class="w-9 h-9 rounded-lg bg-white/10 text-brand-gold flex items-center justify-center shrink-0">
                <i class="fa-solid fa-location-dot"></i>
              </div>
              <div>
                <div class="text-xs text-slate-400">Địa chỉ văn phòng</div>
                <div class="font-medium text-slate-100">Thôn Cẩm Toại Tây, Xã Hòa Vang, TP Đà Nẵng</div>
              </div>
            </div>
          </div>
        </div>

        <!-- Form báo giá -->
        <div class="lg:col-span-7">
          <form id="quoteForm" class="bg-white text-slate-800 rounded-xl p-5 sm:p-7 shadow-lg">
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
              <div>
                <label for="qName" class="block text-xs font-semibold text-slate-700 mb-1.5">Họ và tên *</label>
                <input id="qName" name="name" type="text" required placeholder="Nhập họ tên của bạn" class="w-full px-3.5 py-2.5 rounded-lg border border-slate-300 text-sm focus:outline-none focus:border-brand-gold focus:ring-1 focus:ring-brand-gold" />
              </div>
              <div>
                <label for="qPhone" class="block text-xs font-semibold text-slate-700 mb-1.5">Số điện thoại *</label>
                <input id="qPhone" name="phone" type="tel" required placeholder="Ví dụ: 0934.855.348" class="w-full px-3.5 py-2.5 rounded-lg border border-slate-300 text-sm focus:outline-none focus:border-brand-gold focus:ring-1 focus:ring-brand-gold" />
              </div>
              <div>
                <label for="qEmail" class="block text-xs font-semibold text-slate-700 mb-1.5">Email</label>
                <input id="qEmail" name="email" type="email" placeholder="email@domain.com" class="w-full px-3.5 py-2.5 rounded-lg border border-slate-300 text-sm focus:outline-none focus:border-brand-gold focus:ring-1 focus:ring-brand-gold" />
              </div>
              <div>
                <label for="qType" class="block text-xs font-semibold text-slate-700 mb-1.5">Loại công trình</label>
                <select id="qType" name="type" class="w-full px-3.5 py-2.5 rounded-lg border border-slate-300 text-sm bg-white focus:outline-none focus:border-brand-gold focus:ring-1 focus:ring-brand-gold">
                  <option value="Nhà phố">Nhà phố</option>
                  <option value="Biệt thự">Biệt thự</option>
                  <option value="Khách sạn – Căn hộ cho thuê – Phòng trọ">Khách sạn – Căn hộ cho thuê – Phòng trọ</option>
                  <option value="Văn phòng – Showroom">Văn phòng – Showroom</option>
                  <option value="Cải tạo – Sửa chữa công trình">Cải tạo – Sửa chữa công trình</option>
                  <option value="Công trình hạ tầng – Thủy lợi">Công trình hạ tầng – Thủy lợi</option>
                </select>
              </div>
              <div>
                <label for="qBudget" class="block text-xs font-semibold text-slate-700 mb-1.5">Mức đầu tư dự kiến</label>
                <select id="qBudget" name="budget" class="w-full px-3.5 py-2.5 rounded-lg border border-slate-300 text-sm bg-white focus:outline-none focus:border-brand-gold focus:ring-1 focus:ring-brand-gold">
                  <option value="Chưa xác định">Chưa xác định</option>
                  <option value="Dưới 500 triệu">Dưới 500 triệu</option>
                  <option value="500 triệu – 1 tỷ">500 triệu – 1 tỷ</option>
                  <option value="1 tỷ – 2 tỷ">1 tỷ – 2 tỷ</option>
                  <option value="2 tỷ – 3 tỷ">2 tỷ – 3 tỷ</option>
                  <option value="Trên 3 tỷ">Trên 3 tỷ</option>
                </select>
              </div>
              <div>
                <label for="qService" class="block text-xs font-semibold text-slate-700 mb-1.5">Hạng mục yêu cầu</label>
                <select id="qService" name="service" class="w-full px-3.5 py-2.5 rounded-lg border border-slate-300 text-sm bg-white focus:outline-none focus:border-brand-gold focus:ring-1 focus:ring-brand-gold">
                  <option value="Thi công trọn gói">Thi công trọn gói</option>
                  <option value="Thi công phần thô">Thi công phần thô</option>
                  <option value="Thi công hoàn thiện">Thi công hoàn thiện</option>
                  <option value="Thiết kế kiến trúc – nội thất">Thiết kế kiến trúc – nội thất</option>
                </select>
              </div>
            </div>

            <div class="mt-4">
              <label for="qNote" class="block text-xs font-semibold text-slate-700 mb-1.5">Nội dung yêu cầu (diện tích, số tầng, địa điểm...)</label>
              <textarea id="qNote" name="note" rows="3" placeholder="Mô tả sơ bộ nhu cầu xây dựng của quý khách tại Đà Nẵng..." class="w-full px-3.5 py-2.5 rounded-lg border border-slate-300 text-sm focus:outline-none focus:border-brand-gold focus:ring-1 focus:ring-brand-gold"></textarea>
            </div>

            <div class="mt-5 flex flex-col sm:flex-row sm:items-center justify-between gap-3">
              <button type="submit" class="w-full sm:w-auto px-7 py-3 rounded-lg bg-brand-gold hover:bg-brand-goldDark text-white font-bold text-sm transition-colors shadow">
                Gửi Yêu Cầu Báo Giá
              </button>
              <span class="text-xs text-slate-500">Tây Long Minh cam kết bảo mật thông tin khách hàng.</span>
            </div>

            <!-- Hộp thông báo sau khi gửi form (thay thế alert) -->
            <div id="quoteFeedback" class="hidden mt-4 p-3.5 rounded-lg bg-emerald-50 border border-emerald-200 text-emerald-800 text-xs sm:text-sm font-medium"></div>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- ==================== 10. TIN TỨC & BÀI VIẾT TRANG CHỦ ==================== -->
  <section id="tin-tuc" class="py-10 sm:py-14 bg-white border-t border-slate-200">
    <div class="tlm-container">
      <div class="text-center mb-8">
        <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-tight">Tin Tức &amp; Cẩm Nang Xây Dựng</h2>
        <div class="flatsome-divider mx-auto mt-2.5"></div>
      </div>

      <div id="articlesGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 sm:gap-5"></div>
    </div>
  </section>

  <!-- ==================== 11. DANH MỤC CÁC ĐỐI TÁC TIÊU BIỂU ==================== -->
  <section id="doi-tac" class="py-10 sm:py-12 bg-slate-50 border-t border-slate-200">
    <div class="tlm-container">
      <div class="text-center mb-7">
        <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-tight">Đối Tác &amp; Nhà Cung Cấp Vật Tư</h2>
        <div class="flatsome-divider mx-auto mt-2.5"></div>
      </div>

      <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-6 gap-3 sm:gap-4">
        <!-- Logo đối tác thiết kế SVG rõ nét, đồng bộ -->
        <div class="bg-white rounded-xl border border-slate-200 p-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
          <svg class="h-8 w-auto mb-1.5" viewBox="0 0 140 36" fill="none" xmlns="http://www.w3.org/2000/svg">
            <polygon points="18,4 32,30 4,30" fill="#0F2B4C"/>
            <text x="40" y="24" font-family="Inter, sans-serif" font-weight="800" font-size="14" fill="#0F2B4C">HÒA PHÁT</text>
          </svg>
          <span class="text-[11px] text-slate-500">Thép Xây Dựng</span>
        </div>

        <div class="bg-white rounded-xl border border-slate-200 p-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
          <svg class="h-8 w-auto mb-1.5" viewBox="0 0 140 36" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="4" y="7" width="22" height="22" rx="4" fill="#C88A2E"/>
            <path d="M9 18H21M15 12V24" stroke="#FFF" stroke-width="2.5"/>
            <text x="34" y="24" font-family="Inter, sans-serif" font-weight="800" font-size="14" fill="#0F2B4C">SÔNG GIANH</text>
          </svg>
          <span class="text-[11px] text-slate-500">Xi Măng Chất Lượng</span>
        </div>

        <div class="bg-white rounded-xl border border-slate-200 p-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
          <svg class="h-8 w-auto mb-1.5" viewBox="0 0 140 36" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="16" cy="18" r="11" fill="#0F2B4C"/>
            <text x="34" y="24" font-family="Inter, sans-serif" font-weight="800" font-size="14" fill="#0F2B4C">JOTUN</text>
          </svg>
          <span class="text-[11px] text-slate-500">Sơn Nội Ngoại Thất</span>
        </div>

        <div class="bg-white rounded-xl border border-slate-200 p-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
          <svg class="h-8 w-auto mb-1.5" viewBox="0 0 140 36" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M6 27L16 9L26 27H6Z" stroke="#C88A2E" stroke-width="3" fill="none"/>
            <text x="34" y="24" font-family="Inter, sans-serif" font-weight="800" font-size="14" fill="#0F2B4C">SIKA VN</text>
          </svg>
          <span class="text-[11px] text-slate-500">Chống Thấm &amp; Phụ Gia</span>
        </div>

        <div class="bg-white rounded-xl border border-slate-200 p-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
          <svg class="h-8 w-auto mb-1.5" viewBox="0 0 140 36" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="6" y="8" width="20" height="20" rx="2" stroke="#0F2B4C" stroke-width="3"/>
            <text x="34" y="24" font-family="Inter, sans-serif" font-weight="800" font-size="13" fill="#0F2B4C">VIGLACERA</text>
          </svg>
          <span class="text-[11px] text-slate-500">Gạch &amp; Thiết Bị</span>
        </div>

        <div class="bg-white rounded-xl border border-slate-200 p-4 flex flex-col items-center justify-center text-center hover:border-brand-gold transition-colors">
          <svg class="h-8 w-auto mb-1.5" viewBox="0 0 140 36" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="6" y="10" width="20" height="16" rx="3" fill="#0F2B4C"/>
            <text x="34" y="24" font-family="Inter, sans-serif" font-weight="800" font-size="13.5" fill="#0F2B4C">CADIVI</text>
          </svg>
          <span class="text-[11px] text-slate-500">Thiết Bị Điện Nước</span>
        </div>
      </div>
    </div>
  </section>

  <!-- ==================== 12. GOOGLE MAP & FANPAGE FACEBOOK NGAY NGOÀI TRANG CHỦ ==================== -->
  <section id="lien-he" class="py-10 sm:py-14 bg-white border-t border-slate-200">
    <div class="tlm-container">
      <div class="text-center mb-8">
        <h2 class="text-xl sm:text-2xl font-extrabold text-brand-navy uppercase tracking-tight">
          Bản Đồ Trụ Sở &amp; Kết Nối Fanpage
        </h2>
        <div class="flatsome-divider mx-auto mt-2.5"></div>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-5 sm:gap-6 items-stretch">
        <!-- Cột 1: Google Map trực quan ra ngoài trang chủ -->
        <div class="lg:col-span-7 flex flex-col bg-slate-50 rounded-xl border border-slate-200 overflow-hidden shadow-sm">
          <div class="px-4 py-3 bg-white border-b border-slate-200 flex flex-wrap items-center justify-between gap-2">
            <div class="flex items-center gap-2 text-xs sm:text-sm font-bold text-brand-navy">
              <i class="fa-solid fa-map-location-dot text-brand-gold"></i>
              <span>Thôn Cẩm Toại Tây, Xã Hòa Vang, TP Đà Nẵng</span>
            </div>
            <a href="https://www.google.com/maps/search/?api=1&query=Th%C3%B4n+C%E1%BA%A9m+To%E1%BA%A1i+T%C3%A2y,+X%C3%A3+H%C3%B2a+Vang,+TP+%C4%90%C3%A0+N%E1%BA%B5ng" target="_blank" rel="noopener" class="text-xs font-semibold text-brand-gold hover:underline">
              Mở Google Maps <i class="fa-solid fa-arrow-up-right-from-square ml-0.5 text-[10px]"></i>
            </a>
          </div>
          <div class="w-full h-[300px] sm:h-[340px] flex-1 bg-slate-200">
            <iframe
              title="Bản đồ Công Ty TNHH MTV Tây Long Minh - Thôn Cẩm Toại Tây, Xã Hòa Vang, TP Đà Nẵng"
              src="https://maps.google.com/maps?q=Th%C3%B4n%20C%E1%BA%A9m%20To%E1%BA%A1i%20T%C3%A2y,%20H%C3%B2a%20Vang,%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=15&ie=UTF8&iwloc=&output=embed"
              class="w-full h-full border-0"
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
              allowfullscreen
            ></iframe>
          </div>
        </div>

        <!-- Cột 2: Fanpage Facebook đưa ra ngoài trang chủ -->
        <div id="fanpage-section" class="lg:col-span-5 flex flex-col bg-white rounded-xl border border-slate-200 overflow-hidden shadow-sm">
          <div class="px-4 py-3 bg-white border-b border-slate-200 flex items-center justify-between">
            <div class="flex items-center gap-2 text-xs sm:text-sm font-bold text-brand-navy">
              <i class="fa-brands fa-facebook text-[#1877F2] text-base"></i>
              <span>Fanpage Chính Thức</span>
            </div>
            <span class="text-xs text-slate-500">taylongminh.com</span>
          </div>

          <!-- Khung hiển thị Fanpage Facebook chuyên nghiệp -->
          <div class="p-4 flex-1 flex flex-col justify-between bg-slate-50">
            <div class="bg-white rounded-xl border border-slate-200 overflow-hidden shadow-sm">
              <!-- Ảnh bìa Fanpage -->
              <div class="relative h-32 sm:h-36 bg-brand-navy overflow-hidden">
                <img
                  data-drive-id="1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff"
                  src="https://lh3.googleusercontent.com/d/1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff=w800"
                  alt="Ảnh bìa Fanpage Công Ty TNHH MTV Tây Long Minh"
                  class="w-full h-full object-cover opacity-80"
                />
                <div class="absolute inset-0 bg-gradient-to-t from-black/75 via-black/25 to-transparent"></div>
                <div class="absolute bottom-3 left-3 right-3 flex items-end gap-3">
                  <!-- Avatar Logo Fanpage -->
                  <div class="w-12 h-12 rounded-lg bg-white p-1 shadow shrink-0">
                    <svg class="w-full h-full" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <rect width="64" height="64" rx="10" fill="#0F2B4C"/>
                      <path d="M12 48V24.5L32 11L52 24.5V48H43.5V29L32 21.2L20.5 29V48H12Z" fill="#C88A2E"/>
                      <path d="M25.5 31H38.5V35.5H34.25V48H29.75V35.5H25.5V31Z" fill="#FFFFFF"/>
                    </svg>
                  </div>
                  <div class="min-w-0 text-white">
                    <div class="font-bold text-sm leading-tight truncate">CÔNG TY TNHH MTV TÂY LONG MINH</div>
                    <div class="text-[11px] text-slate-200">Xây dựng &amp; Thiết kế kiến trúc tại Đà Nẵng</div>
                  </div>
                </div>
              </div>

              <!-- Thông tin & Nút tương tác Fanpage -->
              <div class="p-4">
                <p class="text-xs text-slate-600 leading-relaxed mb-3">
                  Cập nhật liên tục hình ảnh tiến độ thi công thực tế, mẫu nhà phố – biệt thự đẹp và ưu đãi xây dựng trọn gói tại Hòa Vang – Đà Nẵng.
                </p>
                <div class="text-xs text-slate-700 space-y-1.5 mb-4">
                  <div class="flex items-center gap-2">
                    <i class="fa-solid fa-phone text-brand-gold w-4"></i>
                    <span>Hotline / Zalo: <strong>0934.855.348</strong></span>
                  </div>
                  <div class="flex items-center gap-2">
                    <i class="fa-solid fa-globe text-brand-gold w-4"></i>
                    <span>Website: <strong>taylongminh.com</strong></span>
                  </div>
                </div>
                <div class="grid grid-cols-2 gap-2.5">
                  <a href="https://www.facebook.com/" target="_blank" rel="noopener" class="inline-flex items-center justify-center gap-1.5 px-3 py-2 rounded-lg bg-[#1877F2] hover:bg-[#1465D1] text-white text-xs font-semibold transition-colors">
                    <i class="fa-brands fa-facebook"></i>
                    <span>Theo dõi Trang</span>
                  </a>
                  <a href="https://m.me/" target="_blank" rel="noopener" class="inline-flex items-center justify-center gap-1.5 px-3 py-2 rounded-lg bg-slate-100 hover:bg-slate-200 text-slate-800 text-xs font-semibold transition-colors">
                    <i class="fa-brands fa-facebook-messenger text-[#0084FF]"></i>
                    <span>Nhắn tin ngay</span>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ==================== 13. FOOTER (FLATSOME STYLE ĐỒNG BỘ MÀU LOGO) ==================== -->
  <footer class="bg-brand-navyDark text-slate-300 pt-10 pb-24 sm:pb-10 border-t-4 border-brand-gold">
    <div class="tlm-container">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 pb-8 border-b border-white/10">
        <!-- Cột 1: Thông tin công ty -->
        <div class="sm:col-span-2 lg:col-span-2">
          <div class="flex items-center gap-2.5 mb-4">
            <svg class="w-9 h-9 shrink-0" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect width="64" height="64" rx="12" fill="#0F2B4C" stroke="#C88A2E" stroke-width="2"/>
              <path d="M12 48V24.5L32 11L52 24.5V48H43.5V29L32 21.2L20.5 29V48H12Z" fill="#C88A2E"/>
              <path d="M25.5 31H38.5V35.5H34.25V48H29.75V35.5H25.5V31Z" fill="#FFFFFF"/>
            </svg>
            <div>
              <div class="text-white font-extrabold text-sm sm:text-base tracking-tight">CÔNG TY TNHH MTV TÂY LONG MINH</div>
              <div class="text-[11px] text-brand-gold font-semibold uppercase tracking-wider">taylongminh.com</div>
            </div>
          </div>
          <ul class="space-y-2 text-xs sm:text-sm text-slate-300">
            <li class="flex items-start gap-2.5">
              <i class="fa-solid fa-location-dot text-brand-gold mt-1"></i>
              <span><strong>Trụ sở:</strong> Thôn Cẩm Toại Tây, Xã Hòa Vang, TP Đà Nẵng</span>
            </li>
            <li class="flex items-center gap-2.5">
              <i class="fa-solid fa-phone text-brand-gold"></i>
              <span><strong>Hotline:</strong> <a href="tel:0934855348" class="text-white hover:text-brand-gold font-semibold">0934.855.348</a></span>
            </li>
            <li class="flex items-center gap-2.5">
              <i class="fa-solid fa-building-columns text-brand-gold"></i>
              <span><strong>Mã số thuế:</strong> 0402185216</span>
            </li>
            <li class="flex items-center gap-2.5">
              <i class="fa-solid fa-globe text-brand-gold"></i>
              <span><strong>Website:</strong> https://taylongminh.com</span>
            </li>
          </ul>
        </div>

        <!-- Cột 2: Lĩnh vực hoạt động -->
        <div>
          <h3 class="text-white font-bold text-sm uppercase tracking-wider mb-3">Lĩnh Vực Hoạt Động</h3>
          <div class="w-10 h-0.5 bg-brand-gold mb-4"></div>
          <ul class="space-y-2 text-xs sm:text-sm">
            <li><a href="#san-pham-thi-cong" onclick="filterProducts('thiet-ke')" class="hover:text-brand-gold transition-colors">Thiết kế kiến trúc – nội thất</a></li>
            <li><a href="#san-pham-thi-cong" onclick="filterProducts('phan-tho')" class="hover:text-brand-gold transition-colors">Thi công phần thô</a></li>
            <li><a href="#san-pham-thi-cong" onclick="filterProducts('hoan-thien')" class="hover:text-brand-gold transition-colors">Thi công hoàn thiện trọn gói</a></li>
            <li><a href="#san-pham-thi-cong" onclick="filterProducts('ha-tang')" class="hover:text-brand-gold transition-colors">Thi công hạ tầng &amp; cải tạo</a></li>
          </ul>
        </div>

        <!-- Cột 3: Danh mục nhanh -->
        <div>
          <h3 class="text-white font-bold text-sm uppercase tracking-wider mb-3">Liên Kết Nhanh</h3>
          <div class="w-10 h-0.5 bg-brand-gold mb-4"></div>
          <ul class="space-y-2 text-xs sm:text-sm">
            <li><a href="#gioi-thieu" class="hover:text-brand-gold transition-colors">Giới thiệu công ty</a></li>
            <li><a href="#du-an-da-nang" class="hover:text-brand-gold transition-colors">Dự án tại Đà Nẵng</a></li>
            <li><a href="#bao-gia" class="hover:text-brand-gold transition-colors">Yêu cầu báo giá</a></li>
            <li><a href="#tin-tuc" class="hover:text-brand-gold transition-colors">Tin tức &amp; Cẩm nang</a></li>
          </ul>
        </div>
      </div>

      <div class="pt-5 text-center text-xs text-slate-400">
        Copyright 2026 © <strong class="text-slate-200">CÔNG TY TNHH MTV TÂY LONG MINH</strong> – taylongminh.com. Bảo lưu mọi quyền.
      </div>
    </div>
  </footer>

  <!-- ==================== 14. CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE - TƯƠNG THÍCH MÁY TÍNH & ĐIỆN THOẠI) ==================== -->
  <div class="fixed right-3 sm:right-5 bottom-4 sm:bottom-6 z-50 flex flex-col gap-2.5 items-end" aria-label="Liên hệ nhanh">
    <!-- Zalo -->
    <a href="https://zalo.me/0934855348" target="_blank" rel="noopener" aria-label="Chat Zalo 0934.855.348" class="group flex items-center gap-2 bg-[#0068FF] hover:bg-[#0055D4] text-white rounded-full shadow-lg p-2.5 sm:px-3.5 sm:py-2.5 transition-all">
      <span class="w-6 h-6 rounded-full bg-white text-[#0068FF] font-extrabold text-[10px] flex items-center justify-center shrink-0">Zalo</span>
      <span class="hidden sm:inline text-xs font-bold pr-1">Chat Zalo</span>
    </a>

    <!-- Facebook -->
    <a href="https://www.facebook.com/" target="_blank" rel="noopener" aria-label="Fanpage Facebook Tây Long Minh" class="group flex items-center gap-2 bg-[#1877F2] hover:bg-[#1465D1] text-white rounded-full shadow-lg p-2.5 sm:px-3.5 sm:py-2.5 transition-all">
      <i class="fa-brands fa-facebook-f w-6 h-6 flex items-center justify-center text-sm shrink-0"></i>
      <span class="hidden sm:inline text-xs font-bold pr-1">Facebook</span>
    </a>

    <!-- Hotline -->
    <a href="tel:0934855348" aria-label="Gọi Hotline 0934.855.348" class="pulse-ring group flex items-center gap-2 bg-brand-gold hover:bg-brand-goldDark text-white rounded-full shadow-lg p-2.5 sm:px-3.5 sm:py-2.5 transition-all">
      <i class="fa-solid fa-phone w-6 h-6 flex items-center justify-center text-sm shrink-0"></i>
      <span class="hidden sm:inline text-xs font-bold pr-1">0934.855.348</span>
    </a>
  </div>

  <!-- ==================== 15. MODAL XEM CHI TIẾT ẢNH CÔNG TRÌNH / BÀI VIẾT ==================== -->
  <div id="detailModal" class="hidden fixed inset-0 z-50 bg-black/70 backdrop-blur-sm flex items-center justify-center p-3 sm:p-5">
    <div class="bg-white rounded-xl max-w-2xl w-full max-h-[90vh] overflow-y-auto shadow-2xl border border-slate-200">
      <div class="sticky top-0 bg-white px-4 sm:px-6 py-3.5 border-b border-slate-200 flex items-center justify-between gap-3 z-10">
        <h3 id="modalTitle" class="text-sm sm:text-base font-bold text-brand-navy leading-snug"></h3>
        <button type="button" onclick="closeModal()" aria-label="Đóng hộp thoại" class="w-8 h-8 rounded-lg bg-slate-100 hover:bg-slate-200 text-slate-700 flex items-center justify-center shrink-0">
          <i class="fa-solid fa-xmark"></i>
        </button>
      </div>
      <div id="modalBody" class="p-4 sm:p-6"></div>
    </div>
  </div>

  <!-- ==================== JAVASCRIPT XỬ LÝ TƯƠNG TÁC & TẢI ẢNH GOOGLE DRIVE ==================== -->
  <script>
    /**
     * Hàm tạo đường dẫn tải ảnh Google Drive tối ưu cùng cơ chế dự phòng đa tầng
     * giúp ảnh thực tế luôn hiển thị mượt mà trên mọi trình duyệt.
     */
    function drivePrimaryUrl(id) {
      return `https://lh3.googleusercontent.com/d/${id}=w1000`;
    }
    function driveSecondaryUrl(id) {
      return `https://drive.google.com/thumbnail?id=${id}&sz=w1000`;
    }
    function handleDriveImageError(imgEl, titleText) {
      const step = imgEl.getAttribute('data-fallback-step') || '0';
      const driveId = imgEl.getAttribute('data-drive-id');
      if (step === '0' && driveId) {
        imgEl.setAttribute('data-fallback-step', '1');
        imgEl.src = driveSecondaryUrl(driveId);
      } else {
        imgEl.onerror = null;
        const encoded = encodeURIComponent(titleText || 'Tây Long Minh');
        imgEl.src = `https://placehold.co/800x600/0F2B4C/FFFFFF?text=${encoded}`;
      }
    }

    // Dữ liệu 9 hạng mục sản phẩm & thi công thực tế (Sử dụng đúng 9 link Google Drive đã cung cấp)
    const productsData = [
      {
        id: 'sp-1',
        driveId: '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz',
        category: 'hoan-thien',
        title: 'Thi Công Xây Dựng Nhà Phố Trọn Gói',
        desc: 'Giải pháp chìa khóa trao tay từ thiết kế, xin phép xây dựng đến thi công phần thô và hoàn thiện nội ngoại thất.'
      },
      {
        id: 'sp-2',
        driveId: '1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR',
        category: 'phan-tho',
        title: 'Thi Công Phần Thô Nhà Ở Dân Dụng',
        desc: 'Thi công móng, kết cấu bê tông cốt thép, xây tô tường đúng tiêu chuẩn kỹ thuật, đảm bảo độ bền vững lâu dài.'
      },
      {
        id: 'sp-3',
        driveId: '1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv',
        category: 'hoan-thien',
        title: 'Thi Công Hoàn Thiện Công Trình Xây Dựng',
        desc: 'Ốp lát gạch, sơn nước, đóng trần thạch cao, lắp đặt cửa nhôm kính và hệ thống điện nước đồng bộ.'
      },
      {
        id: 'sp-4',
        driveId: '1Wlhms5ZB_mL9OptenKvrBS-rGCP2xU1_',
        category: 'thiet-ke',
        title: 'Thiết Kế & Thi Công Biệt Thự Hiện Đại',
        desc: 'Kiến trúc sang trọng, tối ưu ánh sáng tự nhiên và không gian xanh phù hợp khí hậu miền Trung.'
      },
      {
        id: 'sp-5',
        driveId: '1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO',
        category: 'phan-tho',
        title: 'Thi Công Khách Sạn – Căn Hộ Cho Thuê',
        desc: 'Bố trí mặt bằng tối ưu số lượng phòng khai thác, đáp ứng đầy đủ tiêu chuẩn kỹ thuật và phòng cháy chữa cháy.'
      },
      {
        id: 'sp-6',
        driveId: '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t',
        category: 'thiet-ke',
        title: 'Thiết Kế & Thi Công Nội Thất Trọn Gói',
        desc: 'Sản xuất và lắp đặt nội thất gỗ phòng khách, phòng bếp, phòng ngủ tinh tế theo đúng bản vẽ 3D.'
      },
      {
        id: 'sp-7',
        driveId: '1UB12E_spzIvo7TNREjBJXUV9o_HVWOv_',
        category: 'hoan-thien',
        title: 'Xây Dựng Văn Phòng & Không Gian Làm Việc',
        desc: 'Thi công mặt bằng văn phòng chuyên nghiệp, tối ưu công năng sử dụng, tiến độ bàn giao nhanh gọn.'
      },
      {
        id: 'sp-8',
        driveId: '1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT',
        category: 'ha-tang',
        title: 'Thi Công Công Trình Hạ Tầng & Thủy Lợi',
        desc: 'Xây dựng, duy tu sửa chữa kênh mương nội đồng, kè chắn đất và hệ thống thoát nước dân dụng tại Đà Nẵng.'
      },
      {
        id: 'sp-9',
        driveId: '1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn',
        category: 'ha-tang',
        title: 'Cải Tạo Sửa Chữa & San Lấp Mặt Bằng',
        desc: 'Nâng cấp, cải tạo nhà ở cũ, chống thấm triệt để và chuẩn bị san lấp mặt bằng thi công an toàn.'
      }
    ];

    // Dữ liệu 10 dự án thực tế tại Đà Nẵng (Sử dụng đúng 10 link Google Drive đã cung cấp)
    const projectsData = [
      {
        id: 'da-1',
        driveId: '157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT',
        category: 'nha-pho',
        title: 'Nhà Phố Hiện Đại – Hòa Vang, Đà Nẵng',
        location: 'Xã Hòa Vang, TP Đà Nẵng',
        desc: 'Công trình nhà phố gia đình được Tây Long Minh thiết kế và thi công trọn gói với mặt tiền thông thoáng, kết cấu bền chắc.'
      },
      {
        id: 'da-2',
        driveId: '1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff',
        category: 'nha-pho',
        title: 'Nhà Ở Trọn Gói – Hòa Xuân, Đà Nẵng',
        location: 'Khu đô thị Hòa Xuân, Đà Nẵng',
        desc: 'Thi công phần thô và hoàn thiện trọn gói nhà phố 3 tầng, tối ưu không gian sinh hoạt gia đình.'
      },
      {
        id: 'da-3',
        driveId: '1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz',
        category: 'khach-san',
        title: 'Căn Hộ Cho Thuê – Hải Châu, Đà Nẵng',
        location: 'Hải Châu, TP Đà Nẵng',
        desc: 'Xây dựng khối căn hộ dịch vụ cao tầng với hệ thống kỹ thuật điện nước và nội thất đồng bộ.'
      },
      {
        id: 'da-4',
        driveId: '1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k',
        category: 'biet-thu',
        title: 'Biệt Thự 2 Mặt Tiền – Sơn Trà, Đà Nẵng',
        location: 'Sơn Trà, TP Đà Nẵng',
        desc: 'Biệt thự vườn hiện đại kết hợp không gian mở, hoàn thiện tỉ mỉ từng đường nét kiến trúc.'
      },
      {
        id: 'da-5',
        driveId: '1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N',
        category: 'nha-pho',
        title: 'Nhà Phố 3 Tầng – Cẩm Lệ, Đà Nẵng',
        location: 'Cẩm Lệ, TP Đà Nẵng',
        desc: 'Thi công hoàn thiện nhà ở gia đình đúng tiến độ cam kết, vật tư chính hãng minh bạch.'
      },
      {
        id: 'da-6',
        driveId: '1tkQlfZJTkaSunwOIMhfnzkEG2YHwxhML',
        category: 'khach-san',
        title: 'Khách Sạn Lưu Trú – Ngũ Hành Sơn, Đà Nẵng',
        location: 'Ngũ Hành Sơn, TP Đà Nẵng',
        desc: 'Thi công hoàn thiện công trình khách sạn ven biển với tiêu chuẩn kỹ thuật và thẩm mỹ cao.'
      },
      {
        id: 'da-7',
        driveId: '1An7LyMVwj3rhKZlsVnYQ2UrLe48IeTBF',
        category: 'van-phong',
        title: 'Văn Phòng Làm Việc – Thanh Khê, Đà Nẵng',
        location: 'Thanh Khê, TP Đà Nẵng',
        desc: 'Thiết kế và thi công trụ sở văn phòng công ty hiện đại, tối ưu công năng sử dụng.'
      },
      {
        id: 'da-8',
        driveId: '1R1Da04pAYI9-NJz1IsAfa7pVKkuK7J-A',
        category: 'biet-thu',
        title: 'Biệt Thự Gia Đình – Liên Chiểu, Đà Nẵng',
        location: 'Liên Chiểu, TP Đà Nẵng',
        desc: 'Công trình biệt thự sân vườn với hệ mái hiện đại và kết cấu bê tông cốt thép vững chắc.'
      },
      {
        id: 'da-9',
        driveId: '1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80',
        category: 'van-phong',
        title: 'Hạ Tầng Kỹ Thuật – Hòa Vang, Đà Nẵng',
        location: 'Hòa Vang, TP Đà Nẵng',
        desc: 'Hạng mục thi công duy tu, nâng cấp hạ tầng kỹ thuật và kênh tưới nội đồng bảo đảm chất lượng.'
      },
      {
        id: 'da-10',
        driveId: '1So_3V4rw1y7lHegiIkYmh2Z9UIdozAL4',
        category: 'khach-san',
        title: 'Hoàn Thiện Căn Hộ – Nam Việt Á, Đà Nẵng',
        location: 'Khu Nam Việt Á, TP Đà Nẵng',
        desc: 'Thi công hoàn thiện và lắp đặt nội thất căn hộ cao cấp bàn giao chìa khóa trao tay.'
      }
    ];

    // Dữ liệu bài viết trang chủ (tham khảo cấu trúc bài viết từ website mẫu)
    const articlesData = [
      {
        id: 'bv-1',
        driveId: '1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR',
        date: '15/11/2026',
        title: 'Hướng dẫn bảo dưỡng bê tông móng đúng kỹ thuật khi xây nhà',
        excerpt: 'Trong quá trình xây dựng công trình dân dụng, công tác bảo dưỡng bê tông móng quyết định trực tiếp đến cường độ chịu lực và tuổi thọ ngôi nhà.',
        content: 'Sau khi đổ bê tông móng từ 4 đến 6 giờ, cần tiến hành che phủ bằng bạt hoặc bao tải ẩm để tránh mất nước đột ngột dưới nắng gió Đà Nẵng. Trong 7 ngày đầu tiên, cần tưới nước giữ ẩm liên tục từ 3–4 lần mỗi ngày giúp bê tông thủy hóa hoàn toàn, hạn chế rạn nứt chân chim và đạt mác thiết kế chuẩn.'
      },
      {
        id: 'bv-2',
        driveId: '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t',
        date: '10/11/2026',
        title: 'Thiết kế nội thất trọn gói và tầm quan trọng với không gian sống',
        excerpt: 'Bố trí ánh sáng, màu sắc và vật liệu nội thất đồng bộ giúp tối ưu diện tích, tăng sự tiện nghi và tiết kiệm chi phí phát sinh.',
        content: 'Thiết kế nội thất không đơn thuần là sắp đặt bàn ghế hay tủ kệ mà là sự kết hợp hài hòa giữa công năng, luồng di chuyển, thông gió tự nhiên và thẩm mỹ tổng thể. Khi có bản vẽ triển khai chi tiết ngay từ đầu, gia chủ dễ dàng kiểm soát ngân sách và tránh sửa chữa chắp vá về sau.'
      },
      {
        id: 'bv-3',
        driveId: '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz',
        date: '04/11/2026',
        title: '3 lưu ý quan trọng giúp chủ đầu tư xây nhà trọn gói không phát sinh',
        excerpt: 'Chuẩn bị hồ sơ thiết kế đầy đủ, kiểm tra bảng chủng loại vật tư chi tiết và chọn nhà thầu uy tín tại địa phương là 3 yếu tố then chốt.',
        content: 'Để xây nhà không đội chi phí, chủ đầu tư nên chốt kỹ phương án công năng trước khi khởi công, yêu cầu nhà thầu bóc tách rõ ràng từng chủng loại thép, xi măng, dây điện, thiết bị vệ sinh trong phụ lục hợp đồng và thống nhất tiến độ nghiệm thu từng giai đoạn.'
      },
      {
        id: 'bv-4',
        driveId: '1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT',
        date: '28/10/2026',
        title: 'Kinh nghiệm chọn vật liệu chống thấm bền bỉ cho nhà phố miền Trung',
        excerpt: 'Với đặc thù khí hậu nắng nóng và mưa bão lớn tại Đà Nẵng, xử lý chống thấm sàn mái, nhà vệ sinh và tường ngoài cần thực hiện bài bản.',
        content: 'Các vị trí dễ thấm nhất gồm sân thượng, sê-nô, cổ ống xuyên sàn và tường giáp ranh. Tây Long Minh luôn áp dụng quy trình vệ sinh bề mặt, bo góc chân tường, quét 2–3 lớp chống thấm gốc xi măng polymer hoặc màng khò chuyên dụng và ngâm thử nước 48 giờ trước khi lát hoàn thiện.'
      }
    ];

    /**
     * Render danh sách sản phẩm & hạng mục thi công
     * Thiết kế 2 cột trên điện thoại, hiển thị trọn vẹn tên sản phẩm không bị tràn hay mất chữ, không gắn nhãn dán.
     */
    function renderProducts(category = 'all') {
      const container = document.getElementById('productsGrid');
      const filtered = category === 'all'
        ? productsData
        : productsData.filter(item => item.category === category);

      container.innerHTML = filtered.map(item => `
        <article class="bg-white rounded-xl border border-slate-200 overflow-hidden shadow-sm hover:shadow-md transition-all flex flex-col">
          <div class="aspect-[4/3] w-full overflow-hidden bg-slate-100 cursor-pointer" onclick="openItemModal('product', '${item.id}')">
            <img
              data-drive-id="${item.driveId}"
              src="${drivePrimaryUrl(item.driveId)}"
              onerror="handleDriveImageError(this, '${item.title.replace(/'/g, '')}')"
              alt="${item.title}"
              loading="lazy"
              class="w-full h-full object-cover hover:scale-105 transition-transform duration-300"
            />
          </div>
          <div class="p-3 sm:p-4 flex flex-col flex-1 justify-between">
            <div>
              <h3 onclick="openItemModal('product', '${item.id}')" class="text-[13px] sm:text-[15px] font-bold text-brand-navy hover:text-brand-gold transition-colors leading-snug break-words cursor-pointer mb-1.5">
                ${item.title}
              </h3>
              <p class="hidden sm:block text-xs text-slate-600 leading-relaxed mb-3">
                ${item.desc}
              </p>
            </div>
            <div class="pt-2 border-t border-slate-100 flex items-center justify-between gap-2">
              <a href="#bao-gia" class="text-[11.5px] sm:text-xs font-bold text-brand-gold hover:text-brand-navy transition-colors">
                Liên hệ báo giá
              </a>
              <button type="button" onclick="openItemModal('product', '${item.id}')" class="text-[11.5px] sm:text-xs font-semibold text-slate-500 hover:text-brand-navy">
                Chi tiết
              </button>
            </div>
          </div>
        </article>
      `).join('');
    }

    /**
     * Render danh sách 10 dự án tại Đà Nẵng (2 cột trên điện thoại, 5 cột trên desktop)
     */
    function renderProjects(category = 'all') {
      const container = document.getElementById('projectsGrid');
      const filtered = category === 'all'
        ? projectsData
        : projectsData.filter(item => item.category === category);

      container.innerHTML = filtered.map(item => `
        <article class="bg-white rounded-xl border border-slate-200 overflow-hidden shadow-sm hover:shadow-md transition-all flex flex-col">
          <div class="aspect-[4/3] w-full overflow-hidden bg-slate-100 cursor-pointer" onclick="openItemModal('project', '${item.id}')">
            <img
              data-drive-id="${item.driveId}"
              src="${drivePrimaryUrl(item.driveId)}"
              onerror="handleDriveImageError(this, '${item.title.replace(/'/g, '')}')"
              alt="${item.title}"
              loading="lazy"
              class="w-full h-full object-cover hover:scale-105 transition-transform duration-300"
            />
          </div>
          <div class="p-2.5 sm:p-3.5 flex flex-col flex-1 justify-between">
            <h3 onclick="openItemModal('project', '${item.id}')" class="text-[12.5px] sm:text-[13.5px] font-bold text-brand-navy hover:text-brand-gold transition-colors leading-snug break-words cursor-pointer mb-1.5">
              ${item.title}
            </h3>
            <div class="text-[11px] text-slate-500 flex items-center gap-1">
              <i class="fa-solid fa-location-dot text-brand-gold text-[10px] shrink-0"></i>
              <span class="break-words">${item.location}</span>
            </div>
          </div>
        </article>
      `).join('');
    }

    /**
     * Render danh sách bài viết trang chủ
     */
    function renderArticles() {
      const container = document.getElementById('articlesGrid');
      container.innerHTML = articlesData.map(post => `
        <article class="bg-white rounded-xl border border-slate-200 overflow-hidden shadow-sm hover:shadow-md transition-all flex flex-col">
          <div class="aspect-[16/10] w-full overflow-hidden bg-slate-100 cursor-pointer" onclick="openArticleModal('${post.id}')">
            <img
              data-drive-id="${post.driveId}"
              src="${drivePrimaryUrl(post.driveId)}"
              onerror="handleDriveImageError(this, 'Tin tức xây dựng')"
              alt="${post.title}"
              loading="lazy"
              class="w-full h-full object-cover hover:scale-105 transition-transform duration-300"
            />
          </div>
          <div class="p-4 flex flex-col flex-1 justify-between">
            <div>
              <div class="text-[11px] text-slate-400 font-medium mb-1.5">${post.date}</div>
              <h3 onclick="openArticleModal('${post.id}')" class="text-sm font-bold text-brand-navy hover:text-brand-gold transition-colors leading-snug mb-2 cursor-pointer">
                ${post.title}
              </h3>
              <p class="text-xs text-slate-600 leading-relaxed mb-3">
                ${post.excerpt}
              </p>
            </div>
            <button type="button" onclick="openArticleModal('${post.id}')" class="self-start text-xs font-bold text-brand-gold hover:text-brand-navy transition-colors">
              Đọc tiếp <i class="fa-solid fa-arrow-right text-[10px] ml-1"></i>
            </button>
          </div>
        </article>
      `).join('');
    }

    // Bộ lọc tab sản phẩm
    function filterProducts(cat) {
      document.querySelectorAll('.product-tab').forEach(btn => {
        const isActive = btn.getAttribute('data-cat') === cat;
        btn.className = isActive
          ? 'product-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-brand-navy text-white transition-colors'
          : 'product-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-white text-slate-700 border border-slate-200 hover:border-brand-gold transition-colors';
      });
      renderProducts(cat);
    }

    // Bộ lọc tab dự án Đà Nẵng
    function filterProjects(cat) {
      document.querySelectorAll('.project-tab').forEach(btn => {
        const isActive = btn.getAttribute('data-cat') === cat;
        btn.className = isActive
          ? 'project-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-brand-navy text-white transition-colors'
          : 'project-tab cat-no-wrap px-3.5 py-2 rounded-lg text-xs sm:text-[13px] font-semibold bg-slate-100 text-slate-700 hover:bg-brand-goldLight transition-colors';
      });
      renderProjects(cat);
    }

    // Modal xem chi tiết sản phẩm / dự án
    function openItemModal(type, id) {
      const list = type === 'product' ? productsData : projectsData;
      const item = list.find(i => i.id === id);
      if (!item) return;

      document.getElementById('modalTitle').textContent = item.title;
      document.getElementById('modalBody').innerHTML = `
        <div class="rounded-lg overflow-hidden bg-slate-100 mb-4 border border-slate-200">
          <img
            data-drive-id="${item.driveId}"
            src="${drivePrimaryUrl(item.driveId)}"
            onerror="handleDriveImageError(this, '${item.title.replace(/'/g, '')}')"
            alt="${item.title}"
            class="w-full max-h-[380px] object-cover"
          />
        </div>
        ${item.location ? `<p class="text-xs font-semibold text-brand-gold mb-2"><i class="fa-solid fa-location-dot mr-1"></i>${item.location}</p>` : ''}
        <p class="text-sm text-slate-700 leading-relaxed mb-5">${item.desc}</p>
        <div class="flex flex-wrap items-center gap-2.5 pt-3 border-t border-slate-200">
          <a href="tel:0934855348" class="inline-flex items-center gap-2 px-4 py-2.5 rounded-lg bg-brand-navy hover:bg-brand-navyLight text-white text-xs sm:text-sm font-semibold transition-colors">
            <i class="fa-solid fa-phone"></i> Gọi 0934.855.348
          </a>
          <a href="https://zalo.me/0934855348" target="_blank" rel="noopener" class="inline-flex items-center gap-2 px-4 py-2.5 rounded-lg bg-[#0068FF] hover:bg-[#0055D4] text-white text-xs sm:text-sm font-semibold transition-colors">
            Nhắn Zalo tư vấn
          </a>
          <a href="#bao-gia" onclick="closeModal()" class="inline-flex items-center gap-2 px-4 py-2.5 rounded-lg bg-brand-gold hover:bg-brand-goldDark text-white text-xs sm:text-sm font-semibold transition-colors">
            Yêu cầu báo giá
          </a>
        </div>
      `;
      document.getElementById('detailModal').classList.remove('hidden');
    }

    // Modal đọc bài viết
    function openArticleModal(id) {
      const post = articlesData.find(p => p.id === id);
      if (!post) return;
      document.getElementById('modalTitle').textContent = post.title;
      document.getElementById('modalBody').innerHTML = `
        <div class="text-xs text-slate-400 mb-3">Ngày đăng: ${post.date} | CÔNG TY TNHH MTV TÂY LONG MINH</div>
        <div class="rounded-lg overflow-hidden bg-slate-100 mb-4 border border-slate-200">
          <img
            data-drive-id="${post.driveId}"
            src="${drivePrimaryUrl(post.driveId)}"
            onerror="handleDriveImageError(this, 'Bài viết xây dựng')"
            alt="${post.title}"
            class="w-full max-h-[340px] object-cover"
          />
        </div>
        <p class="text-sm text-slate-700 leading-relaxed mb-3">${post.excerpt}</p>
        <p class="text-sm text-slate-700 leading-relaxed mb-5">${post.content}</p>
        <div class="pt-3 border-t border-slate-200 flex items-center justify-between flex-wrap gap-2">
          <span class="text-xs text-slate-500">Cần tư vấn kỹ thuật miễn phí?</span>
          <a href="tel:0934855348" class="px-4 py-2 rounded-lg bg-brand-gold text-white text-xs font-bold hover:bg-brand-goldDark transition-colors">
            Liên hệ: 0934.855.348
          </a>
        </div>
      `;
      document.getElementById('detailModal').classList.remove('hidden');
    }

    function closeModal() {
      document.getElementById('detailModal').classList.add('hidden');
    }

    // Đóng modal khi bấm ra ngoài
    document.getElementById('detailModal').addEventListener('click', function (e) {
      if (e.target === this) closeModal();
    });

    // Điều khiển Hero Slider 2 banner tự trượt (kích thước bằng nhau)
    let currentSlide = 0;
    const slides = document.querySelectorAll('.hero-slide');
    const dots = document.querySelectorAll('.hero-dot');
    let sliderTimer = null;

    function goToSlide(index) {
      currentSlide = (index + slides.length) % slides.length;
      slides.forEach((slide, i) => {
        slide.classList.toggle('active', i === currentSlide);
      });
      dots.forEach((dot, i) => {
        if (i === currentSlide) {
          dot.classList.add('w-6', 'bg-brand-gold');
          dot.classList.remove('w-2.5', 'bg-white/50');
        } else {
          dot.classList.remove('w-6', 'bg-brand-gold');
          dot.classList.add('w-2.5', 'bg-white/50');
        }
      });
    }

    function startAutoSlide() {
      stopAutoSlide();
      sliderTimer = setInterval(() => goToSlide(currentSlide + 1), 5000);
    }

    function stopAutoSlide() {
      if (sliderTimer) clearInterval(sliderTimer);
    }

    document.getElementById('prevSlideBtn').addEventListener('click', () => {
      goToSlide(currentSlide - 1);
      startAutoSlide();
    });

    document.getElementById('nextSlideBtn').addEventListener('click', () => {
      goToSlide(currentSlide + 1);
      startAutoSlide();
    });

    // Hỗ trợ vuốt cảm ứng trên điện thoại cho banner
    let touchStartX = 0;
    const heroContainer = document.getElementById('heroSliderContainer');
    heroContainer.addEventListener('touchstart', (e) => {
      touchStartX = e.changedTouches[0].screenX;
    }, { passive: true });
    heroContainer.addEventListener('touchend', (e) => {
      const diff = e.changedTouches[0].screenX - touchStartX;
      if (Math.abs(diff) > 40) {
        goToSlide(diff > 0 ? currentSlide - 1 : currentSlide + 1);
        startAutoSlide();
      }
    }, { passive: true });

    // Menu mobile đóng/mở
    const mobileMenuBtn = document.getElementById('mobileMenuBtn');
    const mobileMenuPanel = document.getElementById('mobileMenuPanel');
    mobileMenuBtn.addEventListener('click', () => {
      mobileMenuPanel.classList.toggle('hidden');
    });
    function closeMobileMenu() {
      mobileMenuPanel.classList.add('hidden');
    }

    // Gắn fallback cho các ảnh tĩnh dùng Google Drive ID
    document.querySelectorAll('img[data-drive-id]').forEach(img => {
      img.addEventListener('error', function () {
        handleDriveImageError(this, this.alt);
      });
    });

    // Xử lý Form yêu cầu & báo giá (không dùng alert)
    document.getElementById('quoteForm').addEventListener('submit', function (e) {
      e.preventDefault();
      const name = document.getElementById('qName').value.trim();
      const phone = document.getElementById('qPhone').value.trim();
      const type = document.getElementById('qType').value;
      const budget = document.getElementById('qBudget').value;
      const feedback = document.getElementById('quoteFeedback');

      if (!name || !phone) {
        feedback.className = 'mt-4 p-3.5 rounded-lg bg-red-50 border border-red-200 text-red-700 text-xs sm:text-sm font-medium';
        feedback.textContent = 'Vui lòng nhập đầy đủ Họ tên và Số điện thoại để chúng tôi liên hệ tư vấn.';
        feedback.classList.remove('hidden');
        return;
      }

      feedback.className = 'mt-4 p-3.5 rounded-lg bg-emerald-50 border border-emerald-200 text-emerald-800 text-xs sm:text-sm font-medium';
      feedback.innerHTML = `<i class="fa-solid fa-circle-check mr-1.5"></i> Cảm ơn <strong>${name}</strong>! Yêu cầu báo giá công trình <strong>${type}</strong> (mức đầu tư: ${budget}) đã được gửi đến <strong>CÔNG TY TNHH MTV TÂY LONG MINH</strong>. Chúng tôi sẽ gọi lại số <strong>${phone}</strong> trong thời gian sớm nhất.`;
      feedback.classList.remove('hidden');
      this.reset();
    });

    // Khởi tạo giao diện ban đầu
    renderProducts('all');
    renderProjects('all');
    renderArticles();
    startAutoSlide();
  </script>
</body>
</html>
