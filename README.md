<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>آراد پرداخت - درگاه پرداخت و خدمات مالی</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            box-sizing: border-box;
        }
        
        @import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;600;700&display=swap');
        
        * {
            font-family: 'Vazirmatn', sans-serif;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #0f0f0f 0%, #1a1a1a 50%, #0f0f0f 100%);
        }
        
        .gold-gradient {
            background: linear-gradient(135deg, #d4af37 0%, #ffd700 50%, #d4af37 100%);
        }
        
        .card-hover {
            transition: all 0.4s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 25px 35px -5px rgba(212, 175, 55, 0.3);
        }
        
        .fade-in {
            animation: fadeIn 0.6s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .slide-in {
            animation: slideIn 0.4s ease-out;
        }
        
        @keyframes slideIn {
            from { transform: translateX(100%); }
            to { transform: translateX(0); }
        }
        
        .arad-logo {
            background: linear-gradient(45deg, #d4af37, #ffd700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-weight: bold;
            font-size: 1.5rem;
        }
        
        .gold-text {
            color: #d4af37;
        }
        
        .gold-border {
            border-color: #d4af37;
        }
        
        .service-modal {
            backdrop-filter: blur(10px);
            background: rgba(0, 0, 0, 0.8);
        }
        
        .service-card {
            background: linear-gradient(145deg, #1a1a1a, #0f0f0f);
            border: 1px solid rgba(212, 175, 55, 0.2);
        }
        
        .service-card:hover {
            border-color: rgba(212, 175, 55, 0.5);
            box-shadow: 0 0 30px rgba(212, 175, 55, 0.2);
        }
        
        .category-tab {
            background: linear-gradient(145deg, #2a2a2a, #1a1a1a);
            border: 1px solid rgba(212, 175, 55, 0.3);
        }
        
        .category-tab.active {
            background: linear-gradient(145deg, #d4af37, #ffd700);
            color: #000;
            box-shadow: 0 5px 15px rgba(212, 175, 55, 0.4);
        }
        
        .license-badge {
            background: linear-gradient(145deg, #d4af37, #ffd700);
            color: #000;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
        }
        
        .price-tag {
            background: linear-gradient(145deg, #1a1a1a, #0f0f0f);
            border: 2px solid #d4af37;
            border-radius: 10px;
            padding: 8px 16px;
        }
        
        .stats-card {
            background: linear-gradient(145deg, #1a1a1a, #0f0f0f);
            border: 1px solid rgba(212, 175, 55, 0.3);
            backdrop-filter: blur(10px);
        }
        
        .api-code {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 16px;
            font-family: 'Courier New', monospace;
            color: #c9d1d9;
            overflow-x: auto;
        }
        
        .testimonial-card {
            background: linear-gradient(145deg, #1a1a1a, #0f0f0f);
            border: 1px solid rgba(212, 175, 55, 0.2);
            backdrop-filter: blur(10px);
        }
        
        .floating-element {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        .pulse-glow {
            animation: pulseGlow 2s ease-in-out infinite alternate;
        }
        
        @keyframes pulseGlow {
            from { box-shadow: 0 0 20px rgba(212, 175, 55, 0.3); }
            to { box-shadow: 0 0 40px rgba(212, 175, 55, 0.6); }
        }
        
        .mobile-menu {
            transform: translateX(100%);
            transition: transform 0.3s ease;
        }
        
        .mobile-menu.open {
            transform: translateX(0);
        }
        
        .counter {
            font-variant-numeric: tabular-nums;
        }
        
        .gradient-text {
            background: linear-gradient(135deg, #d4af37, #ffd700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .glass-effect {
            background: rgba(26, 26, 26, 0.8);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(212, 175, 55, 0.2);
        }
        
        .progress-bar {
            background: linear-gradient(90deg, #d4af37, #ffd700);
            height: 4px;
            border-radius: 2px;
            transition: width 0.3s ease;
        }
        
        .notification-dot {
            width: 8px;
            height: 8px;
            background: #ef4444;
            border-radius: 50%;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.5; }
        }
    </style>
</head>
<body class="bg-black text-white">
    <!-- Navigation -->
    <nav class="bg-gradient-to-r from-black to-gray-900 shadow-2xl sticky top-0 z-50 border-b-2 border-yellow-600">
        <div class="max-w-7xl mx-auto px-4">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center space-x-4 space-x-reverse">
                    <div class="flex items-center">
                        <!-- Arad Logo -->
                        <div class="w-12 h-12 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-xl flex items-center justify-center shadow-xl pulse-glow">
                            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M12 2L2 7L12 12L22 7L12 2Z" fill="#000"/>
                                <path d="M2 17L12 22L22 17" stroke="#000" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M2 12L12 17L22 12" stroke="#000" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                            </svg>
                        </div>
                        <span class="mr-3 text-2xl font-bold arad-logo">آراد پرداخت</span>
                    </div>
                </div>
                
                <div class="hidden md:flex items-center space-x-6 space-x-reverse">
                    <a href="#" onclick="showSection('home')" class="text-gray-300 hover:text-yellow-400 transition-colors font-medium relative">
                        خانه
                        <div class="notification-dot absolute -top-1 -right-1"></div>
                    </a>
                    <a href="#" onclick="showSection('services')" class="text-gray-300 hover:text-yellow-400 transition-colors font-medium">خدمات</a>
                    <a href="#" onclick="showSection('licenses')" class="text-gray-300 hover:text-yellow-400 transition-colors font-medium">مجوزها</a>
                    <a href="#" onclick="showSection('api')" class="text-gray-300 hover:text-yellow-400 transition-colors font-medium">API</a>
                    <a href="#" onclick="showSection('about')" class="text-gray-300 hover:text-yellow-400 transition-colors font-medium">درباره ما</a>
                    <a href="#" onclick="showSection('contact')" class="text-gray-300 hover:text-yellow-400 transition-colors font-medium">تماس</a>
                </div>
                
                <div class="flex items-center space-x-3 space-x-reverse">
                    <button onclick="showSection('login')" class="text-yellow-400 hover:text-yellow-300 font-medium">ورود</button>
                    <button onclick="showSection('register')" class="bg-gradient-to-r from-yellow-400 to-yellow-600 text-black px-6 py-2 rounded-xl hover:from-yellow-500 hover:to-yellow-700 transition-all font-medium shadow-lg">ثبت نام</button>
                    
                    <!-- Mobile Menu Button -->
                    <button onclick="toggleMobileMenu()" class="md:hidden text-yellow-400">
                        <svg width="24" height="24" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile Menu -->
        <div id="mobileMenu" class="mobile-menu fixed top-0 right-0 h-full w-64 bg-black border-l border-yellow-600 z-50 md:hidden">
            <div class="p-4">
                <div class="flex justify-between items-center mb-8">
                    <span class="text-xl font-bold arad-logo">آراد پرداخت</span>
                    <button onclick="toggleMobileMenu()" class="text-yellow-400">✕</button>
                </div>
                <nav class="space-y-4">
                    <a href="#" onclick="showSection('home'); toggleMobileMenu()" class="block text-gray-300 hover:text-yellow-400 py-2">خانه</a>
                    <a href="#" onclick="showSection('services'); toggleMobileMenu()" class="block text-gray-300 hover:text-yellow-400 py-2">خدمات</a>
                    <a href="#" onclick="showSection('licenses'); toggleMobileMenu()" class="block text-gray-300 hover:text-yellow-400 py-2">مجوزها</a>
                    <a href="#" onclick="showSection('api'); toggleMobileMenu()" class="block text-gray-300 hover:text-yellow-400 py-2">API</a>
                    <a href="#" onclick="showSection('about'); toggleMobileMenu()" class="block text-gray-300 hover:text-yellow-400 py-2">درباره ما</a>
                    <a href="#" onclick="showSection('contact'); toggleMobileMenu()" class="block text-gray-300 hover:text-yellow-400 py-2">تماس</a>
                </nav>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <div id="content">
        <!-- Home Section -->
        <section id="home" class="section-content">
            <!-- Hero Section -->
            <div class="gradient-bg text-white py-24 relative overflow-hidden">
                <div class="absolute inset-0 bg-gradient-to-r from-yellow-400/10 to-transparent"></div>
                
                <!-- Floating Elements -->
                <div class="absolute top-20 left-10 w-20 h-20 bg-yellow-400/20 rounded-full floating-element"></div>
                <div class="absolute top-40 right-20 w-16 h-16 bg-yellow-600/30 rounded-full floating-element" style="animation-delay: -2s;"></div>
                <div class="absolute bottom-20 left-1/4 w-12 h-12 bg-yellow-500/25 rounded-full floating-element" style="animation-delay: -4s;"></div>
                
                <div class="max-w-7xl mx-auto px-4 text-center relative z-10">
                    <h1 class="text-7xl font-bold mb-8 fade-in">
                        <span class="arad-logo">آراد پرداخت</span>
                    </h1>
                    <p class="text-2xl mb-10 opacity-90 fade-in">درگاه پرداخت مطمئن و خدمات مالی پیشرفته با امنیت بالا</p>
                    
                    <!-- Stats Counter -->
                    <div class="grid grid-cols-2 md:grid-cols-4 gap-6 mb-12 fade-in">
                        <div class="stats-card rounded-xl p-6">
                            <div class="text-3xl font-bold gold-text counter" data-target="50000">0</div>
                            <div class="text-gray-400">کاربر فعال</div>
                        </div>
                        <div class="stats-card rounded-xl p-6">
                            <div class="text-3xl font-bold gold-text counter" data-target="1000000">0</div>
                            <div class="text-gray-400">تراکنش موفق</div>
                        </div>
                        <div class="stats-card rounded-xl p-6">
                            <div class="text-3xl font-bold gold-text counter" data-target="99">0</div>
                            <div class="text-gray-400">درصد آپتایم</div>
                        </div>
                        <div class="stats-card rounded-xl p-6">
                            <div class="text-3xl font-bold gold-text counter" data-target="24">0</div>
                            <div class="text-gray-400">ساعته پشتیبانی</div>
                        </div>
                    </div>
                    
                    <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-6 sm:space-x-reverse fade-in">
                        <button onclick="showSection('register')" class="bg-gradient-to-r from-yellow-400 to-yellow-600 text-black px-10 py-4 rounded-xl font-bold hover:from-yellow-500 hover:to-yellow-700 transition-all shadow-2xl text-lg">شروع کنید</button>
                        <button onclick="showSection('services')" class="border-2 border-yellow-400 text-yellow-400 px-10 py-4 rounded-xl font-bold hover:bg-yellow-400 hover:text-black transition-all text-lg">خدمات ما</button>
                    </div>
                </div>
            </div>

            <!-- Features -->
            <div class="py-24 bg-gradient-to-b from-gray-900 to-black">
                <div class="max-w-7xl mx-auto px-4">
                    <h2 class="text-4xl font-bold text-center text-white mb-16">ویژگی‌های <span class="gold-text">آراد پرداخت</span></h2>
                    <div class="grid md:grid-cols-3 gap-10">
                        <div class="text-center p-8 card-hover service-card rounded-2xl">
                            <div class="w-20 h-20 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center mx-auto mb-6">
                                <span class="text-3xl text-black">💳</span>
                            </div>
                            <h3 class="text-2xl font-bold mb-4 gold-text">پرداخت امن</h3>
                            <p class="text-gray-400 text-lg">پرداخت‌های آنلاین با بالاترین سطح امنیت و رمزنگاری</p>
                            <div class="progress-bar mt-4" style="width: 95%"></div>
                        </div>
                        
                        <div class="text-center p-8 card-hover service-card rounded-2xl">
                            <div class="w-20 h-20 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center mx-auto mb-6">
                                <span class="text-3xl text-black">🔄</span>
                            </div>
                            <h3 class="text-2xl font-bold mb-4 gold-text">انتقال سریع</h3>
                            <p class="text-gray-400 text-lg">انتقال فوری پول بین حساب‌ها و کیف پول‌های مختلف</p>
                            <div class="progress-bar mt-4" style="width: 98%"></div>
                        </div>
                        
                        <div class="text-center p-8 card-hover service-card rounded-2xl">
                            <div class="w-20 h-20 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center mx-auto mb-6">
                                <span class="text-3xl text-black">📊</span>
                            </div>
                            <h3 class="text-2xl font-bold mb-4 gold-text">پنل مدیریت</h3>
                            <p class="text-gray-400 text-lg">پنل مدیریت پیشرفته با گزارش‌گیری کامل و نظارت</p>
                            <div class="progress-bar mt-4" style="width: 92%"></div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Testimonials -->
            <div class="py-24 bg-gradient-to-b from-black to-gray-900">
                <div class="max-w-7xl mx-auto px-4">
                    <h2 class="text-4xl font-bold text-center text-white mb-16">نظرات <span class="gold-text">مشتریان</span></h2>
                    <div class="grid md:grid-cols-3 gap-8">
                        <div class="testimonial-card rounded-2xl p-8">
                            <div class="flex items-center mb-4">
                                <div class="w-12 h-12 bg-yellow-400 rounded-full flex items-center justify-center ml-4">
                                    <span class="text-black font-bold">ع</span>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white">علی احمدی</h4>
                                    <p class="text-gray-400 text-sm">مدیر فروش</p>
                                </div>
                            </div>
                            <p class="text-gray-300">"سرویس عالی و پشتیبانی فوق‌العاده. تراکنش‌ها خیلی سریع انجام میشه و امنیت بالایی داره."</p>
                            <div class="flex mt-4">
                                <span class="text-yellow-400">★★★★★</span>
                            </div>
                        </div>
                        
                        <div class="testimonial-card rounded-2xl p-8">
                            <div class="flex items-center mb-4">
                                <div class="w-12 h-12 bg-yellow-400 rounded-full flex items-center justify-center ml-4">
                                    <span class="text-black font-bold">م</span>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white">مریم کریمی</h4>
                                    <p class="text-gray-400 text-sm">صاحب کسب‌وکار</p>
                                </div>
                            </div>
                            <p class="text-gray-300">"API خیلی راحت و مستندات کاملی داره. تو کمتر از یک روز تونستم پیاده‌سازی کنم."</p>
                            <div class="flex mt-4">
                                <span class="text-yellow-400">★★★★★</span>
                            </div>
                        </div>
                        
                        <div class="testimonial-card rounded-2xl p-8">
                            <div class="flex items-center mb-4">
                                <div class="w-12 h-12 bg-yellow-400 rounded-full flex items-center justify-center ml-4">
                                    <span class="text-black font-bold">ح</span>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white">حسن رضایی</h4>
                                    <p class="text-gray-400 text-sm">توسعه‌دهنده</p>
                                </div>
                            </div>
                            <p class="text-gray-300">"کارمزدهای منصفانه و سرویس پایدار. از زمانی که شروع کردم هیچ مشکلی نداشتم."</p>
                            <div class="flex mt-4">
                                <span class="text-yellow-400">★★★★★</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="section-content hidden">
            <div class="py-20 bg-gradient-to-b from-black to-gray-900">
                <div class="max-w-7xl mx-auto px-4">
                    <h2 class="text-4xl font-bold text-center text-white mb-16">خدمات <span class="gold-text">آراد پرداخت</span></h2>
                    
                    <!-- Service Categories Tabs -->
                    <div class="flex flex-wrap justify-center gap-4 mb-12">
                        <button onclick="showServiceCategory('customer')" class="category-tab px-6 py-3 rounded-xl font-medium transition-all active">خدمات مشتری</button>
                        <button onclick="showServiceCategory('account')" class="category-tab px-6 py-3 rounded-xl font-medium transition-all">خدمات حساب</button>
                        <button onclick="showServiceCategory('transfer')" class="category-tab px-6 py-3 rounded-xl font-medium transition-all">انتقال وجه</button>
                        <button onclick="showServiceCategory('card')" class="category-tab px-6 py-3 rounded-xl font-medium transition-all">خدمات کارت</button>
                        <button onclick="showServiceCategory('check')" class="category-tab px-6 py-3 rounded-xl font-medium transition-all">چک و تسهیلات</button>
                        <button onclick="showServiceCategory('insurance')" class="category-tab px-6 py-3 rounded-xl font-medium transition-all">بیمه و هویت</button>
                    </div>

                    <!-- Customer Services -->
                    <div id="customer-services" class="service-category">
                        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('customer-info')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">👤</span>
                                    <h3 class="text-xl font-bold gold-text">اطلاعات مشتری</h3>
                                </div>
                                <p class="text-gray-400 mb-4">مشاهده و ویرایش اطلاعات شخصی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">رایگان</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('inquiry-services')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🔍</span>
                                    <h3 class="text-xl font-bold gold-text">استعلامات</h3>
                                </div>
                                <p class="text-gray-400 mb-4">استعلام موجودی، تراکنش و سایر خدمات</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۵۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('token-management')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🔐</span>
                                    <h3 class="text-xl font-bold gold-text">مدیریت توکن</h3>
                                </div>
                                <p class="text-gray-400 mb-4">ایجاد و مدیریت توکن‌های امنیتی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۱,۰۰۰ ریال</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Account Services -->
                    <div id="account-services" class="service-category hidden">
                        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('account-management')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🏦</span>
                                    <h3 class="text-xl font-bold gold-text">مدیریت حساب</h3>
                                </div>
                                <p class="text-gray-400 mb-4">مدیریت کامل حساب‌های بانکی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۲,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('account-block')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🚫</span>
                                    <h3 class="text-xl font-bold gold-text">مسدودی حساب</h3>
                                </div>
                                <p class="text-gray-400 mb-4">مسدود و رفع مسدودی حساب</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۵,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('direct-debit')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">⚡</span>
                                    <h3 class="text-xl font-bold gold-text">برداشت مستقیم</h3>
                                </div>
                                <p class="text-gray-400 mb-4">تنظیم برداشت خودکار از حساب</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۱,۵۰۰ ریال</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Transfer Services -->
                    <div id="transfer-services" class="service-category hidden">
                        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('internal-transfer')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🔄</span>
                                    <h3 class="text-xl font-bold gold-text">انتقال درون بانکی</h3>
                                </div>
                                <p class="text-gray-400 mb-4">انتقال وجه بین حساب‌های یک بانک</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۱,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('paya-transfer')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">💸</span>
                                    <h3 class="text-xl font-bold gold-text">انتقال پایا</h3>
                                </div>
                                <p class="text-gray-400 mb-4">انتقال وجه از طریق سیستم پایا</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۳,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('satna-transfer')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">⚡</span>
                                    <h3 class="text-xl font-bold gold-text">انتقال ساتنا</h3>
                                </div>
                                <p class="text-gray-400 mb-4">انتقال فوری از طریق سیستم ساتنا</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۵,۰۰۰ ریال</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Card Services -->
                    <div id="card-services" class="service-category hidden">
                        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('card-management')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">💳</span>
                                    <h3 class="text-xl font-bold gold-text">مدیریت کارت</h3>
                                </div>
                                <p class="text-gray-400 mb-4">مدیریت کامل کارت‌های بانکی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۲,۵۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('card-to-card')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🔄</span>
                                    <h3 class="text-xl font-bold gold-text">کارت به کارت</h3>
                                </div>
                                <p class="text-gray-400 mb-4">انتقال وجه بین کارت‌ها</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۱,۵۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('bill-payment')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🧾</span>
                                    <h3 class="text-xl font-bold gold-text">پرداخت قبض</h3>
                                </div>
                                <p class="text-gray-400 mb-4">پرداخت انواع قبوض</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۵۰۰ ریال</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Check Services -->
                    <div id="check-services" class="service-category hidden">
                        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('check-management')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">📝</span>
                                    <h3 class="text-xl font-bold gold-text">مدیریت چک</h3>
                                </div>
                                <p class="text-gray-400 mb-4">صدور و مدیریت چک‌ها</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۳,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('sayad-check')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🛡️</span>
                                    <h3 class="text-xl font-bold gold-text">چک صیاد</h3>
                                </div>
                                <p class="text-gray-400 mb-4">صدور چک صیاد تضمینی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۱۰,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('facilities')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">💰</span>
                                    <h3 class="text-xl font-bold gold-text">تسهیلات</h3>
                                </div>
                                <p class="text-gray-400 mb-4">دریافت انواع تسهیلات بانکی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۰.۵% از مبلغ</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Insurance Services -->
                    <div id="insurance-services" class="service-category hidden">
                        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('social-insurance')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🏥</span>
                                    <h3 class="text-xl font-bold gold-text">بیمه تامین اجتماعی</h3>
                                </div>
                                <p class="text-gray-400 mb-4">خدمات بیمه تامین اجتماعی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۲,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('identity-verification')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">🆔</span>
                                    <h3 class="text-xl font-bold gold-text">احراز هویت</h3>
                                </div>
                                <p class="text-gray-400 mb-4">تایید هویت و اعتبارسنجی</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۵,۰۰۰ ریال</span>
                                </div>
                            </div>

                            <div class="service-card rounded-2xl p-6 card-hover cursor-pointer" onclick="showServiceDetail('mobile-services')">
                                <div class="flex items-center mb-4">
                                    <span class="text-3xl ml-4">📱</span>
                                    <h3 class="text-xl font-bold gold-text">خدمات موبایل</h3>
                                </div>
                                <p class="text-gray-400 mb-4">شارژ و بسته‌های اینترنت</p>
                                <div class="price-tag">
                                    <span class="text-yellow-400 font-bold">۱% کارمزد</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Licenses Section -->
        <section id="licenses" class="section-content hidden">
            <div class="py-20 bg-gradient-to-b from-gray-900 to-black">
                <div class="max-w-7xl mx-auto px-4">
                    <h2 class="text-4xl font-bold text-center text-white mb-16">مجوزها و <span class="gold-text">گواهینامه‌ها</span></h2>
                    
                    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                        <!-- Central Bank License -->
                        <div class="service-card rounded-2xl p-8 text-center card-hover">
                            <div class="w-24 h-24 mx-auto mb-6 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center">
                                <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M12 2L2 7L12 12L22 7L12 2Z" fill="#000"/>
                                    <path d="M2 17L12 22L22 17" stroke="#000" stroke-width="2"/>
                                    <path d="M2 12L12 17L22 12" stroke="#000" stroke-width="2"/>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold gold-text mb-4">مجوز بانک مرکزی</h3>
                            <p class="text-gray-400 mb-4">مجوز رسمی ارائه خدمات پرداخت از بانک مرکزی جمهوری اسلامی ایران</p>
                            <div class="license-badge">شماره مجوز: PSP-2023-001</div>
                        </div>

                        <!-- Security Certificate -->
                        <div class="service-card rounded-2xl p-8 text-center card-hover">
                            <div class="w-24 h-24 mx-auto mb-6 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center">
                                <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z" fill="#000"/>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold gold-text mb-4">گواهی امنیت ISO 27001</h3>
                            <p class="text-gray-400 mb-4">استاندارد بین‌المللی مدیریت امنیت اطلاعات</p>
                            <div class="license-badge">ISO 27001:2013</div>
                        </div>

                        <!-- PCI DSS -->
                        <div class="service-card rounded-2xl p-8 text-center card-hover">
                            <div class="w-24 h-24 mx-auto mb-6 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center">
                                <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <rect x="2" y="3" width="20" height="14" rx="2" ry="2" fill="#000"/>
                                    <line x1="2" y1="9" x2="22" y2="9" stroke="#d4af37" stroke-width="2"/>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold gold-text mb-4">گواهی PCI DSS</h3>
                            <p class="text-gray-400 mb-4">استاندارد امنیت داده‌های کارت پرداخت</p>
                            <div class="license-badge">PCI DSS Level 1</div>
                        </div>

                        <!-- Digital Trust -->
                        <div class="service-card rounded-2xl p-8 text-center card-hover">
                            <div class="w-24 h-24 mx-auto mb-6 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center">
                                <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" stroke="#000" stroke-width="2" fill="none"/>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold gold-text mb-4">نماد اعتماد الکترونیک</h3>
                            <p class="text-gray-400 mb-4">تایید صحت و اعتبار از مرکز توسعه تجارت الکترونیک</p>
                            <div class="license-badge">eNamad Verified</div>
                        </div>

                        <!-- GDPR Compliance -->
                        <div class="service-card rounded-2xl p-8 text-center card-hover">
                            <div class="w-24 h-24 mx-auto mb-6 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center">
                                <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z" fill="#000"/>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold gold-text mb-4">تطبیق با GDPR</h3>
                            <p class="text-gray-400 mb-4">رعایت قوانین حفاظت از داده‌های شخصی اروپا</p>
                            <div class="license-badge">GDPR Compliant</div>
                        </div>

                        <!-- API Security -->
                        <div class="service-card rounded-2xl p-8 text-center card-hover">
                            <div class="w-24 h-24 mx-auto mb-6 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center">
                                <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M13 10V3L4 14h7v7l9-11h-7z" fill="#000"/>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold gold-text mb-4">امنیت API</h3>
                            <p class="text-gray-400 mb-4">گواهی امنیت و پایداری سرویس‌های API</p>
                            <div class="license-badge">OAuth 2.0 & JWT</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- API Section -->
        <section id="api" class="section-content hidden">
            <div class="py-20 bg-gradient-to-b from-black to-gray-900">
                <div class="max-w-7xl mx-auto px-4">
                    <h2 class="text-4xl font-bold text-center text-white mb-16">مستندات <span class="gold-text">API</span></h2>
                    
                    <div class="grid lg:grid-cols-2 gap-12">
                        <!-- API Info -->
                        <div>
                            <h3 class="text-2xl font-bold gold-text mb-6">شروع سریع</h3>
                            <p class="text-gray-300 mb-8">API آراد پرداخت امکان پیاده‌سازی آسان پرداخت‌های آنلاین را فراهم می‌کند. با استفاده از RESTful API ما می‌توانید در کمتر از ۳۰ دقیقه سیستم پرداخت خود را راه‌اندازی کنید.</p>
                            
                            <div class="space-y-6">
                                <div class="glass-effect rounded-xl p-6">
                                    <h4 class="text-lg font-bold text-white mb-3">🚀 راه‌اندازی سریع</h4>
                                    <p class="text-gray-400">تنها با چند خط کد، سیستم پرداخت خود را فعال کنید</p>
                                </div>
                                
                                <div class="glass-effect rounded-xl p-6">
                                    <h4 class="text-lg font-bold text-white mb-3">🔒 امنیت بالا</h4>
                                    <p class="text-gray-400">رمزنگاری AES-256 و پروتکل‌های امنیتی پیشرفته</p>
                                </div>
                                
                                <div class="glass-effect rounded-xl p-6">
                                    <h4 class="text-lg font-bold text-white mb-3">📊 گزارش‌گیری کامل</h4>
                                    <p class="text-gray-400">دسترسی به گزارش‌های تفصیلی و آمار تراکنش‌ها</p>
                                </div>
                            </div>
                        </div>
                        
                        <!-- Code Example -->
                        <div>
                            <h3 class="text-2xl font-bold gold-text mb-6">نمونه کد</h3>
                            
                            <div class="api-code mb-6">
                                <div class="text-sm text-gray-400 mb-2">// ایجاد درخواست پرداخت</div>
                                <pre class="text-green-400">
curl -X POST https://api.aradpay.ir/v1/payment \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "amount": 100000,
    "currency": "IRR",
    "callback_url": "https://yoursite.com/callback",
    "description": "خرید محصول"
  }'</pre>
                            </div>
                            
                            <div class="api-code mb-6">
                                <div class="text-sm text-gray-400 mb-2">// پاسخ API</div>
                                <pre class="text-blue-400">
{
  "status": "success",
  "payment_id": "pay_1234567890",
  "payment_url": "https://pay.aradpay.ir/gateway/pay_1234567890",
  "expires_at": "2024-01-01T12:00:00Z"
}</pre>
                            </div>
                            
                            <div class="flex space-x-4 space-x-reverse">
                                <button onclick="showToast('مستندات کامل در حال آماده‌سازی است')" class="bg-gradient-to-r from-yellow-400 to-yellow-600 text-black px-6 py-3 rounded-xl font-bold hover:from-yellow-500 hover:to-yellow-700 transition-all">
                                    مستندات کامل
                                </button>
                                <button onclick="showToast('کلید API تست ارسال شد')" class="border-2 border-yellow-400 text-yellow-400 px-6 py-3 rounded-xl font-bold hover:bg-yellow-400 hover:text-black transition-all">
                                    کلید تست
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="section-content hidden">
            <div class="py-20 bg-gradient-to-b from-gray-900 to-black">
                <div class="max-w-7xl mx-auto px-4">
                    <h2 class="text-4xl font-bold text-center text-white mb-16">درباره <span class="gold-text">آراد پرداخت</span></h2>
                    
                    <div class="grid lg:grid-cols-2 gap-12 items-center">
                        <div>
                            <h3 class="text-3xl font-bold gold-text mb-6">پیشرو در خدمات پرداخت</h3>
                            <p class="text-gray-300 text-lg mb-6">
                                آراد پرداخت با بیش از ۱۰ سال تجربه در حوزه خدمات مالی و پرداخت الکترونیک، یکی از معتبرترین ارائه‌دهندگان خدمات پرداخت در کشور محسوب می‌شود.
                            </p>
                            <p class="text-gray-300 text-lg mb-8">
                                ما با ارائه راه‌حل‌های نوآورانه و امن، به کسب‌وکارها کمک می‌کنیم تا فرآیند پرداخت خود را بهینه‌سازی کرده و تجربه بهتری برای مشتریان خود فراهم کنند.
                            </p>
                            
                            <div class="grid grid-cols-2 gap-6">
                                <div class="text-center">
                                    <div class="text-3xl font-bold gold-text counter" data-target="10">0</div>
                                    <div class="text-gray-400">سال تجربه</div>
                                </div>
                                <div class="text-center">
                                    <div class="text-3xl font-bold gold-text counter" data-target="500">0</div>
                                    <div class="text-gray-400">کسب‌وکار فعال</div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="space-y-6">
                            <div class="glass-effect rounded-xl p-6">
                                <h4 class="text-xl font-bold gold-text mb-3">🎯 ماموریت ما</h4>
                                <p class="text-gray-300">ارائه خدمات پرداخت امن، سریع و قابل اعتماد برای تمامی کسب‌وکارها</p>
                            </div>
                            
                            <div class="glass-effect rounded-xl p-6">
                                <h4 class="text-xl font-bold gold-text mb-3">👁️ چشم‌انداز ما</h4>
                                <p class="text-gray-300">تبدیل شدن به پیشروترین پلتفرم پرداخت در منطقه خاورمیانه</p>
                            </div>
                            
                            <div class="glass-effect rounded-xl p-6">
                                <h4 class="text-xl font-bold gold-text mb-3">⚡ ارزش‌های ما</h4>
                                <p class="text-gray-300">امنیت، شفافیت، نوآوری و خدمات مشتری‌محور</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="section-content hidden">
            <div class="py-20 bg-gradient-to-b from-black to-gray-900">
                <div class="max-w-7xl mx-auto px-4">
                    <h2 class="text-4xl font-bold text-center text-white mb-16">تماس با <span class="gold-text">ما</span></h2>
                    
                    <div class="grid lg:grid-cols-2 gap-12">
                        <!-- Contact Form -->
                        <div>
                            <h3 class="text-2xl font-bold gold-text mb-6">پیام خود را ارسال کنید</h3>
                            <form id="contactForm" class="space-y-6">
                                <div class="grid grid-cols-2 gap-4">
                                    <div>
                                        <label class="block text-sm font-medium text-gray-300 mb-2">نام</label>
                                        <input type="text" required class="w-full px-4 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="نام شما">
                                    </div>
                                    <div>
                                        <label class="block text-sm font-medium text-gray-300 mb-2">نام خانوادگی</label>
                                        <input type="text" required class="w-full px-4 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="نام خانوادگی">
                                    </div>
                                </div>
                                
                                <div>
                                    <label class="block text-sm font-medium text-gray-300 mb-2">ایمیل</label>
                                    <input type="email" required class="w-full px-4 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="example@email.com">
                                </div>
                                
                                <div>
                                    <label class="block text-sm font-medium text-gray-300 mb-2">شماره تماس</label>
                                    <input type="tel" required class="w-full px-4 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="09123456789">
                                </div>
                                
                                <div>
                                    <label class="block text-sm font-medium text-gray-300 mb-2">موضوع</label>
                                    <select required class="w-full px-4 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white">
                                        <option value="">انتخاب کنید</option>
                                        <option value="support">پشتیبانی فنی</option>
                                        <option value="sales">فروش و مشاوره</option>
                                        <option value="partnership">همکاری</option>
                                        <option value="other">سایر موارد</option>
                                    </select>
                                </div>
                                
                                <div>
                                    <label class="block text-sm font-medium text-gray-300 mb-2">پیام</label>
                                    <textarea required rows="5" class="w-full px-4 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white resize-none" placeholder="پیام خود را بنویسید..."></textarea>
                                </div>
                                
                                <button type="submit" class="w-full bg-gradient-to-r from-yellow-400 to-yellow-600 text-black py-3 rounded-lg hover:from-yellow-500 hover:to-yellow-700 transition-all font-medium">
                                    ارسال پیام
                                </button>
                            </form>
                        </div>
                        
                        <!-- Contact Info -->
                        <div class="space-y-8">
                            <div>
                                <h3 class="text-2xl font-bold gold-text mb-6">اطلاعات تماس</h3>
                                
                                <div class="space-y-6">
                                    <div class="glass-effect rounded-xl p-6">
                                        <div class="flex items-center">
                                            <div class="w-12 h-12 bg-yellow-400 rounded-full flex items-center justify-center ml-4">
                                                <span class="text-black text-xl">📍</span>
                                            </div>
                                            <div>
                                                <h4 class="font-bold text-white">آدرس دفتر مرکزی</h4>
                                                <p class="text-gray-400">تهران، خیابان ولیعصر، پلاک ۱۲۳۴</p>
                                            </div>
                                        </div>
                                    </div>
                                    
                                    <div class="glass-effect rounded-xl p-6">
                                        <div class="flex items-center">
                                            <div class="w-12 h-12 bg-yellow-400 rounded-full flex items-center justify-center ml-4">
                                                <span class="text-black text-xl">📞</span>
                                            </div>
                                            <div>
                                                <h4 class="font-bold text-white">تلفن پشتیبانی</h4>
                                                <p class="text-gray-400">۰۲۱-۱۲۳۴۵۶۷۸</p>
                                            </div>
                                        </div>
                                    </div>
                                    
                                    <div class="glass-effect rounded-xl p-6">
                                        <div class="flex items-center">
                                            <div class="w-12 h-12 bg-yellow-400 rounded-full flex items-center justify-center ml-4">
                                                <span class="text-black text-xl">✉️</span>
                                            </div>
                                            <div>
                                                <h4 class="font-bold text-white">ایمیل</h4>
                                                <p class="text-gray-400">info@aradpay.ir</p>
                                            </div>
                                        </div>
                                    </div>
                                    
                                    <div class="glass-effect rounded-xl p-6">
                                        <div class="flex items-center">
                                            <div class="w-12 h-12 bg-yellow-400 rounded-full flex items-center justify-center ml-4">
                                                <span class="text-black text-xl">🕒</span>
                                            </div>
                                            <div>
                                                <h4 class="font-bold text-white">ساعات کاری</h4>
                                                <p class="text-gray-400">شنبه تا پنج‌شنبه: ۸ تا ۱۸</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <div>
                                <h4 class="text-xl font-bold gold-text mb-4">شبکه‌های اجتماعی</h4>
                                <div class="flex space-x-4 space-x-reverse">
                                    <a href="#" class="w-12 h-12 bg-gray-700 rounded-full flex items-center justify-center hover:bg-yellow-400 hover:text-black transition-all">
                                        <span>📱</span>
                                    </a>
                                    <a href="#" class="w-12 h-12 bg-gray-700 rounded-full flex items-center justify-center hover:bg-yellow-400 hover:text-black transition-all">
                                        <span>💬</span>
                                    </a>
                                    <a href="#" class="w-12 h-12 bg-gray-700 rounded-full flex items-center justify-center hover:bg-yellow-400 hover:text-black transition-all">
                                        <span>📧</span>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Login Section -->
        <section id="login" class="section-content hidden">
            <div class="min-h-screen flex items-center justify-center bg-black py-12 px-4">
                <div class="max-w-md w-full space-y-8">
                    <div class="text-center">
                        <div class="w-16 h-16 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center mx-auto mb-4 pulse-glow">
                            <span class="text-black font-bold text-2xl">آ</span>
                        </div>
                        <h2 class="text-3xl font-bold text-white">ورود به حساب</h2>
                        <p class="mt-2 text-gray-400">به آراد پرداخت خوش آمدید</p>
                    </div>
                    
                    <form id="loginForm" class="mt-8 space-y-6">
                        <div>
                            <label class="block text-sm font-medium text-gray-300 mb-1">شماره موبایل یا ایمیل</label>
                            <input type="text" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="09123456789">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium text-gray-300 mb-1">رمز عبور</label>
                            <input type="password" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="رمز عبور خود را وارد کنید">
                        </div>
                        
                        <div class="flex items-center justify-between">
                            <label class="flex items-center">
                                <input type="checkbox" class="rounded border-gray-600 text-yellow-500 focus:ring-yellow-500">
                                <span class="mr-2 text-gray-400 text-sm">مرا به خاطر بسپار</span>
                            </label>
                            <a href="#" class="text-yellow-400 hover:text-yellow-300 text-sm">فراموشی رمز عبور؟</a>
                        </div>
                        
                        <button type="submit" class="w-full bg-gradient-to-r from-yellow-400 to-yellow-600 text-black py-3 rounded-lg hover:from-yellow-500 hover:to-yellow-700 transition-all font-medium">
                            ورود
                        </button>
                        
                        <div class="text-center">
                            <span class="text-gray-400">حساب کاربری ندارید؟ </span>
                            <button type="button" onclick="showSection('register')" class="text-yellow-400 hover:text-yellow-300 font-medium">ثبت نام کنید</button>
                        </div>
                    </form>
                </div>
            </div>
        </section>

        <!-- Register Section -->
        <section id="register" class="section-content hidden">
            <div class="min-h-screen flex items-center justify-center bg-black py-12 px-4">
                <div class="max-w-md w-full space-y-8">
                    <div class="text-center">
                        <div class="w-16 h-16 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full flex items-center justify-center mx-auto mb-4 pulse-glow">
                            <span class="text-black font-bold text-2xl">آ</span>
                        </div>
                        <h2 class="text-3xl font-bold text-white">ثبت نام</h2>
                        <p class="mt-2 text-gray-400">حساب جدید ایجاد کنید</p>
                    </div>
                    
                    <form id="registerForm" class="mt-8 space-y-6">
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-300 mb-1">نام</label>
                                <input type="text" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="نام">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-300 mb-1">نام خانوادگی</label>
                                <input type="text" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="نام خانوادگی">
                            </div>
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium text-gray-300 mb-1">شماره موبایل</label>
                            <input type="tel" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="09123456789">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium text-gray-300 mb-1">ایمیل</label>
                            <input type="email" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="example@email.com">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium text-gray-300 mb-1">رمز عبور</label>
                            <input type="password" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="رمز عبور قوی انتخاب کنید">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium text-gray-300 mb-1">تکرار رمز عبور</label>
                            <input type="password" required class="w-full px-3 py-3 bg-gray-800 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500 text-white" placeholder="رمز عبور را مجدداً وارد کنید">
                        </div>
                        
                        <div class="flex items-center">
                            <input type="checkbox" required class="rounded border-gray-600 text-yellow-500 focus:ring-yellow-500">
                            <span class="mr-2 text-gray-400 text-sm">با <a href="#" class="text-yellow-400 hover:text-yellow-300">قوانین و مقررات</a> موافقم</span>
                        </div>
                        
                        <button type="submit" class="w-full bg-gradient-to-r from-yellow-400 to-yellow-600 text-black py-3 rounded-lg hover:from-yellow-500 hover:to-yellow-700 transition-all font-medium">
                            ثبت نام
                        </button>
                        
                        <div class="text-center">
                            <span class="text-gray-400">قبلاً ثبت نام کرده‌اید؟ </span>
                            <button type="button" onclick="showSection('login')" class="text-yellow-400 hover:text-yellow-300 font-medium">وارد شوید</button>
                        </div>
                    </form>
                </div>
            </div>
        </section>
    </div>

    <!-- Service Detail Modal -->
    <div id="serviceModal" class="fixed inset-0 service-modal hidden items-center justify-center z-50">
        <div class="bg-gradient-to-br from-gray-900 to-black rounded-2xl p-8 w-full max-w-2xl mx-4 slide-in border-2 border-yellow-600">
            <div class="flex justify-between items-center mb-6">
                <h3 id="serviceTitle" class="text-2xl font-bold gold-text"></h3>
                <button onclick="closeServiceModal()" class="text-gray-400 hover:text-gray-300 text-2xl">✕</button>
            </div>
            
            <div id="serviceContent" class="space-y-6">
                <!-- Content will be populated by JavaScript -->
            </div>
        </div>
    </div>

    <!-- Success Toast -->
    <div id="successToast" class="fixed top-4 left-4 bg-gradient-to-r from-yellow-400 to-yellow-600 text-black px-6 py-3 rounded-lg shadow-lg hidden z-50">
        <div class="flex items-center">
            <span class="ml-2">✓</span>
            <span id="successMessage">عملیات با موفقیت انجام شد</span>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-gradient-to-r from-black to-gray-900 border-t-2 border-yellow-600 py-12">
        <div class="max-w-7xl mx-auto px-4">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center mb-4">
                        <div class="w-10 h-10 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-lg flex items-center justify-center ml-3">
                            <span class="text-black font-bold">آ</span>
                        </div>
                        <span class="text-xl font-bold arad-logo">آراد پرداخت</span>
                    </div>
                    <p class="text-gray-400 mb-4">درگاه پرداخت مطمئن و خدمات مالی پیشرفته</p>
                    <div class="flex space-x-3 space-x-reverse">
                        <a href="#" class="w-8 h-8 bg-gray-700 rounded-full flex items-center justify-center hover:bg-yellow-400 hover:text-black transition-all">
                            <span class="text-sm">📱</span>
                        </a>
                        <a href="#" class="w-8 h-8 bg-gray-700 rounded-full flex items-center justify-center hover:bg-yellow-400 hover:text-black transition-all">
                            <span class="text-sm">💬</span>
                        </a>
                        <a href="#" class="w-8 h-8 bg-gray-700 rounded-full flex items-center justify-center hover:bg-yellow-400 hover:text-black transition-all">
                            <span class="text-sm">📧</span>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold text-white mb-4">خدمات</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">درگاه پرداخت</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">انتقال وجه</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">کیف پول</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">API پرداخت</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold text-white mb-4">پشتیبانی</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">مرکز راهنمایی</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">تماس با ما</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">گزارش مشکل</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">وضعیت سرویس</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold text-white mb-4">شرکت</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">درباره ما</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">اخبار</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">فرصت‌های شغلی</a></li>
                        <li><a href="#" class="hover:text-yellow-400 transition-colors">قوانین و مقررات</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; ۱۴۰۳ آراد پرداخت. تمامی حقوق محفوظ است.</p>
            </div>
        </div>
    </footer>

    <script>
        // Service details data
        const serviceDetails = {
            'customer-info': {
                title: 'اطلاعات مشتری',
                icon: '👤',
                description: 'مشاهده و ویرایش کامل اطلاعات شخصی و حساب کاربری',
                price: 'رایگان',
                commission: 'بدون کارمزد',
                features: [
                    'مشاهده اطلاعات شخصی',
                    'ویرایش اطلاعات تماس',
                    'تغییر رمز عبور',
                    'مدیریت تنظیمات امنیتی',
                    'تاریخچه فعالیت‌ها'
                ],
                subServices: [
                    { name: 'مشاهده پروفایل', price: 'رایگان' },
                    { name: 'ویرایش اطلاعات', price: 'رایگان' },
                    { name: 'تغییر رمز عبور', price: 'رایگان' },
                    { name: 'تنظیمات امنیتی', price: 'رایگان' }
                ]
            },
            'inquiry-services': {
                title: 'خدمات استعلام',
                icon: '🔍',
                description: 'استعلام موجودی، تراکنش‌ها و سایر اطلاعات حساب',
                price: '۵۰۰ ریال',
                commission: '۵۰۰ ریال به ازای هر استعلام',
                features: [
                    'استعلام موجودی حساب',
                    'استعلام تراکنش‌ها',
                    'استعلام وضعیت چک',
                    'استعلام قبوض',
                    'گزارش‌گیری تفصیلی'
                ],
                subServices: [
                    { name: 'استعلام موجودی', price: '۵۰۰ ریال' },
                    { name: 'استعلام تراکنش', price: '۷۰۰ ریال' },
                    { name: 'استعلام چک', price: '۱,۰۰۰ ریال' },
                    { name: 'استعلام قبض', price: '۳۰۰ ریال' }
                ]
            },
            'token-management': {
                title: 'مدیریت توکن',
                icon: '🔐',
                description: 'ایجاد، مدیریت و تمدید توکن‌های امنیتی برای دسترسی به API',
                price: '۱,۰۰۰ ریال',
                commission: '۱,۰۰۰ ریال برای هر توکن',
                features: [
                    'ایجاد توکن جدید',
                    'مدیریت دسترسی‌ها',
                    'تمدید توکن‌ها',
                    'حذف توکن‌های منقضی',
                    'نظارت بر استفاده'
                ],
                subServices: [
                    { name: 'ایجاد توکن', price: '۱,۰۰۰ ریال' },
                    { name: 'تمدید توکن', price: '۵۰۰ ریال' },
                    { name: 'حذف توکن', price: 'رایگان' },
                    { name: 'مدیریت دسترسی', price: '۲۰۰ ریال' }
                ]
            },
            'account-management': {
                title: 'مدیریت حساب',
                icon: '🏦',
                description: 'مدیریت کامل حساب‌های بانکی و تنظیمات مربوطه',
                price: '۲,۰۰۰ ریال',
                commission: '۲,۰۰۰ ریال برای هر عملیات',
                features: [
                    'افتتاح حساب جدید',
                    'بستن حساب',
                    'تغییر نوع حساب',
                    'مدیریت امضای مجاز',
                    'تنظیم حد اعتبار'
                ],
                subServices: [
                    { name: 'افتتاح حساب', price: '۵,۰۰۰ ریال' },
                    { name: 'بستن حساب', price: '۳,۰۰۰ ریال' },
                    { name: 'تغییر نوع حساب', price: '۲,۰۰۰ ریال' },
                    { name: 'مدیریت امضا', price: '۱,۵۰۰ ریال' }
                ]
            },
            'internal-transfer': {
                title: 'انتقال درون بانکی',
                icon: '🔄',
                description: 'انتقال وجه بین حساب‌های یک بانک با سرعت بالا',
                price: '۱,۰۰۰ ریال',
                commission: '۱,۰۰۰ ریال + ۰.۱% از مبلغ',
                features: [
                    'انتقال فوری',
                    'بدون محدودیت مبلغ',
                    'تایید SMS',
                    'ردیابی تراکنش',
                    'گزارش‌گیری'
                ],
                subServices: [
                    { name: 'انتقال عادی', price: '۱,۰۰۰ ریال' },
                    { name: 'انتقال فوری', price: '۲,۰۰۰ ریال' },
                    { name: 'انتقال برنامه‌ریزی شده', price: '۱,۵۰۰ ریال' },
                    { name: 'انتقال گروهی', price: '۵۰۰ ریال هر مورد' }
                ]
            }
        };

        // Counter animation
        function animateCounters() {
            const counters = document.querySelectorAll('.counter');
            counters.forEach(counter => {
                const target = parseInt(counter.getAttribute('data-target'));
                const increment = target / 100;
                let current = 0;
                
                const timer = setInterval(() => {
                    current += increment;
                    if (current >= target) {
                        counter.textContent = target.toLocaleString();
                        clearInterval(timer);
                    } else {
                        counter.textContent = Math.floor(current).toLocaleString();
                    }
                }, 20);
            });
        }

        // Mobile menu toggle
        function toggleMobileMenu() {
            const mobileMenu = document.getElementById('mobileMenu');
            mobileMenu.classList.toggle('open');
        }

        // Navigation
        function showSection(sectionId) {
            const sections = document.querySelectorAll('.section-content');
            sections.forEach(section => {
                section.classList.add('hidden');
            });
            
            const targetSection = document.getElementById(sectionId);
            if (targetSection) {
                targetSection.classList.remove('hidden');
                targetSection.classList.add('fade-in');
                
                // Animate counters when home section is shown
                if (sectionId === 'home') {
                    setTimeout(animateCounters, 500);
                }
            }
        }

        // Service Category Navigation
        function showServiceCategory(categoryId) {
            // Hide all service categories
            const categories = document.querySelectorAll('.service-category');
            categories.forEach(category => {
                category.classList.add('hidden');
            });
            
            // Remove active class from all tabs
            const tabs = document.querySelectorAll('.category-tab');
            tabs.forEach(tab => {
                tab.classList.remove('active');
            });
            
            // Show target category
            const targetCategory = document.getElementById(categoryId + '-services');
            if (targetCategory) {
                targetCategory.classList.remove('hidden');
            }
            
            // Add active class to clicked tab
            event.target.classList.add('active');
        }

        // Show Service Detail Modal
        function showServiceDetail(serviceId) {
            const service = serviceDetails[serviceId];
            if (!service) return;

            const modal = document.getElementById('serviceModal');
            const title = document.getElementById('serviceTitle');
            const content = document.getElementById('serviceContent');

            title.textContent = service.title;
            
            content.innerHTML = `
                <div class="flex items-center mb-6">
                    <span class="text-4xl ml-4">${service.icon}</span>
                    <div>
                        <h4 class="text-xl font-bold text-white">${service.title}</h4>
                        <p class="text-gray-400">${service.description}</p>
                    </div>
                </div>

                <div class="grid md:grid-cols-2 gap-6 mb-6">
                    <div class="price-tag">
                        <h5 class="font-bold text-yellow-400 mb-2">قیمت پایه</h5>
                        <p class="text-white text-lg">${service.price}</p>
                    </div>
                    <div class="price-tag">
                        <h5 class="font-bold text-yellow-400 mb-2">کارمزد</h5>
                        <p class="text-white text-lg">${service.commission}</p>
                    </div>
                </div>

                <div class="mb-6">
                    <h5 class="font-bold text-yellow-400 mb-3">ویژگی‌ها</h5>
                    <ul class="space-y-2">
                        ${service.features.map(feature => `
                            <li class="flex items-center text-gray-300">
                                <span class="text-yellow-400 ml-2">✓</span>
                                ${feature}
                            </li>
                        `).join('')}
                    </ul>
                </div>

                <div class="mb-6">
                    <h5 class="font-bold text-yellow-400 mb-3">زیرمجموعه خدمات</h5>
                    <div class="grid gap-3">
                        ${service.subServices.map(subService => `
                            <div class="flex justify-between items-center p-3 bg-gray-800 rounded-lg border border-gray-700">
                                <span class="text-white">${subService.name}</span>
                                <span class="text-yellow-400 font-bold">${subService.price}</span>
                            </div>
                        `).join('')}
                    </div>
                </div>

                <div class="flex space-x-4 space-x-reverse">
                    <button onclick="requestService('${serviceId}')" class="flex-1 bg-gradient-to-r from-yellow-400 to-yellow-600 text-black py-3 rounded-xl font-bold hover:from-yellow-500 hover:to-yellow-700 transition-all">
                        درخواست خدمت
                    </button>
                    <button onclick="closeServiceModal()" class="flex-1 bg-gray-700 text-white py-3 rounded-xl font-bold hover:bg-gray-600 transition-all">
                        بستن
                    </button>
                </div>
            `;

            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        // Close Service Modal
        function closeServiceModal() {
            const modal = document.getElementById('serviceModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        // Request Service
        function requestService(serviceId) {
            const service = serviceDetails[serviceId];
            showToast(`درخواست ${service.title} با موفقیت ثبت شد`);
            closeServiceModal();
        }

        // Toast notification
        function showToast(message, type = 'success') {
            const toast = document.getElementById('successToast');
            const messageEl = document.getElementById('successMessage');
            
            messageEl.textContent = message;
            toast.classList.remove('hidden');
            
            setTimeout(() => {
                toast.classList.add('hidden');
            }, 3000);
        }

        // Form handlers
        document.getElementById('loginForm').addEventListener('submit', function(e) {
            e.preventDefault();
            showToast('ورود موفقیت‌آمیز بود');
        });

        document.getElementById('registerForm').addEventListener('submit', function(e) {
            e.preventDefault();
            showToast('ثبت نام با موفقیت انجام شد');
        });

        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            showToast('پیام شما با موفقیت ارسال شد');
        });

        // Close modal when clicking outside
        document.addEventListener('click', function(e) {
            if (e.target.id === 'serviceModal') {
                closeServiceModal();
            }
            if (e.target.id === 'mobileMenu') {
                toggleMobileMenu();
            }
        });

        // Initialize
        document.addEventListener('DOMContentLoaded', function() {
            showSection('home');
            setTimeout(animateCounters, 1000);
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9893435e51389125',t:'MTc1OTU2NjA1OS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
