<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MS Shoe Hub – Premium Footwear & Accessories, Hyderabad</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');
        
        :root { --primary: #000000; }
        
        * { font-family: 'Inter', system-ui, sans-serif; }
        
        .logo-text {
            font-size: 2.8rem;
            line-height: 1;
            font-weight: 900;
            letter-spacing: -4px;
        }
        
        .hero-bg {
            background: linear-gradient(rgba(0, 0, 0, 0.65), rgba(0, 0, 0, 0.65)), url('https://picsum.photos/id/1015/1920/1080') center/cover no-repeat;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .product-card {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
        }
        
        .product-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            left: 0;
            background-color: #000;
            transition: all 0.3s;
        }
        
        .nav-link:hover:after { width: 100%; }
        
        .category-pill {
            transition: all 0.3s;
            cursor: pointer;
        }
        
        .category-pill:hover {
            border-color: #000;
            transform: translateY(-2px);
        }

        /* FIX: Image loading fallback */
        img {
            background-color: #f3f4f6;
        }

        /* FIX: Mobile menu improvements */
        @media (max-width: 768px) {
            .logo-text {
                font-size: 1.8rem;
            }
            
            nav {
                flex-wrap: wrap;
                gap: 0.5rem !important;
            }
        }
    </style>
</head>
<body class="bg-gray-50">

    <!-- HEADER -->
    <header class="bg-white border-b sticky top-0 z-50 shadow-sm">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex items-center justify-between py-5 flex-wrap gap-4">
                <!-- Logo -->
                <div class="flex flex-col items-center -space-y-2">
                    <div class="logo-text text-black">M S</div>
                    <div class="logo-text text-black">S H O E</div>
                    <div class="logo-text text-black">H U B</div>
                </div>

                <!-- Location & Tagline - Hidden on mobile -->
                <div class="hidden md:block text-center">
                    <div class="text-sm font-medium text-gray-500">Falaknuma · Hyderabad</div>
                    <div class="text-xs font-semibold tracking-widest text-black">Premium Quality Since 2025</div>
                </div>

                <!-- Navigation -->
                <nav class="flex items-center gap-8 text-sm font-semibold flex-wrap">
                    <a href="#" class="nav-link text-black hover:text-gray-700">Home</a>
                    <a href="#collections" class="nav-link text-black hover:text-gray-700">Collections</a>
                    <a href="#about" class="nav-link text-black hover:text-gray-700">About Us</a>
                    
                    <!-- WhatsApp Button -->
                    <a href="https://wa.me/919177784328?text=Hello%20MS%20SHOE%20HUB!%20I%20would%20like%20to%20book%20a%20product.%20Bookings%20accepted%20only%20on%20%2B919177784328" 
                       target="_blank"
                       rel="noopener noreferrer"
                       class="flex items-center gap-2 bg-green-600 hover:bg-green-700 text-white px-4 md:px-6 py-2 md:py-3 rounded-3xl text-xs md:text-sm font-semibold transition-colors whitespace-nowrap">
                        <i class="fab fa-whatsapp text-lg"></i>
                        <span class="hidden sm:inline">+91 91777 84328</span>
                    </a>
                </nav>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="hero-bg text-white relative">
        <div class="max-w-4xl mx-auto px-6 py-16 md:py-28 text-center w-full">
            <h1 class="text-5xl md:text-7xl font-black tracking-tighter mb-4">MS SHOE HUB</h1>
            <p class="text-xl md:text-2xl font-medium mb-2">Premium Quality Since 2025</p>
            <p class="text-2xl md:text-4xl font-light max-w-2xl mx-auto mb-10 px-4">
                Experience unmatched comfort with our premium collection of sleepers. 
                <br class="hidden md:block">Crafted for style, designed for comfort.
            </p>
            <div class="flex flex-col md:flex-row flex-wrap justify-center gap-4 px-4">
                <a href="#collections" 
                   class="px-8 md:px-10 py-4 md:py-5 bg-white text-black font-semibold rounded-3xl text-base md:text-lg hover:bg-amber-400 transition-colors">
                    Explore Collections
                </a>
                <a href="https://wa.me/919177784328?text=Hello%20MS%20SHOE%20HUB!%20I%20would%20like%20to%20book%20a%20product." 
                   target="_blank"
                   rel="noopener noreferrer"
                   class="px-8 md:px-10 py-4 md:py-5 border-2 border-white font-semibold rounded-3xl text-base md:text-lg hover:bg-white hover:text-black transition-colors">
                    Chat on WhatsApp
                </a>
            </div>
            <div class="mt-12 md:mt-16 text-sm flex items-center justify-center gap-2 text-white/70">
                <div class="w-3 h-px bg-white/70"></div>
                SCROLL FOR MORE
                <div class="w-3 h-px bg-white/70"></div>
            </div>
        </div>
    </section>

    <!-- COLLECTIONS SECTION -->
    <section id="collections" class="max-w-7xl mx-auto px-6 py-16">
        <div class="text-center mb-12">
            <h2 class="text-4xl md:text-5xl font-bold tracking-tight">Shop By Category</h2>
        </div>

        <!-- Category Pills -->
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4 mb-16">
            <a href="#womens" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Women's Sleepers & Slippers</a>
            <a href="#mens-loafers" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Men's Loafers & Boots</a>
            <a href="#araba" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Araba Slippers</a>
            <a href="#dailywear" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Daily Wear Slippers</a>
            <a href="#underwear" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Men's Underwear</a>
            <a href="#banyans" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Men's Banyans</a>
            <a href="#kids" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Kids Sleepers</a>
            <a href="#accessories" class="category-pill bg-white border border-gray-200 hover:border-black rounded-3xl px-6 py-6 text-center font-medium text-sm md:text-base">Accessories</a>
        </div>

        <!-- ARABA SLIPPERS SECTION -->
        <div id="araba" class="mb-20 scroll-mt-20">
            <div class="flex flex-col md:flex-row justify-between md:items-end gap-4 mb-8">
                <div>
                    <h2 class="text-3xl md:text-4xl font-bold">Araba Slippers</h2>
                    <p class="text-gray-600 text-sm md:text-base">Premium comfort for men • ₹399–₹599</p>
                </div>
                <a href="#" class="text-black font-medium flex items-center gap-2 hover:gap-3 transition-all text-sm md:text-base">View All <i class="fas fa-arrow-right"></i></a>
            </div>
            <div id="araba-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-4 md:gap-6"></div>
        </div>

        <!-- DAILY WEAR SLIPPERS SECTION -->
        <div id="dailywear" class="mb-20 scroll-mt-20">
            <div class="flex flex-col md:flex-row justify-between md:items-end gap-4 mb-8">
                <div>
                    <h2 class="text-3xl md:text-4xl font-bold">Daily Wear Slippers for Men</h2>
                    <p class="text-gray-600 text-sm md:text-base">Fixed Price ₹499</p>
                </div>
                <a href="#" class="text-black font-medium flex items-center gap-2 hover:gap-3 transition-all text-sm md:text-base">View All <i class="fas fa-arrow-right"></i></a>
            </div>
            <div id="daily-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-4 md:gap-6"></div>
        </div>

        <!-- MEN'S UNDERWEAR SECTION -->
        <div id="underwear" class="mb-20 scroll-mt-20">
            <div class="flex flex-col md:flex-row justify-between md:items-end gap-4 mb-8">
                <div>
                    <h2 class="text-3xl md:text-4xl font-bold">Men's Underwear</h2>
                    <p class="text-gray-600 text-sm md:text-base">Premium comfort & style • Dixcy Scott</p>
                </div>
                <a href="#" class="text-black font-medium flex items-center gap-2 hover:gap-3 transition-all text-sm md:text-base">View All <i class="fas fa-arrow-right"></i></a>
            </div>
            <div id="underwear-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-4 md:gap-6"></div>
        </div>

        <!-- MEN'S BANYANS SECTION -->
        <div id="banyans" class="mb-20 scroll-mt-20">
            <div class="flex flex-col md:flex-row justify-between md:items-end gap-4 mb-8">
                <div>
                    <h2 class="text-3xl md:text-4xl font-bold">Men's Banyans</h2>
                    <p class="text-gray-600 text-sm md:text-base">Premium vests & banians • Rupa & Essa</p>
                </div>
                <a href="#" class="text-black font-medium flex items-center gap-2 hover:gap-3 transition-all text-sm md:text-base">View All <i class="fas fa-arrow-right"></i></a>
            </div>
            <div id="banyans-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-4 md:gap-6"></div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-black text-white py-12 md:py-16">
        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-12 gap-8 md:gap-10">
            <div class="md:col-span-5">
                <div class="flex flex-col items-start -space-y-2 mb-6">
                    <div class="logo-text text-white text-3xl md:text-4xl">M S</div>
                    <div class="logo-text text-white text-3xl md:text-4xl">S H O E</div>
                    <div class="logo-text text-white text-3xl md:text-4xl">H U B</div>
                </div>
                <p class="text-gray-400 max-w-xs text-sm md:text-base">Premium footwear &amp; accessories in the heart of Hyderabad since 2025.</p>
                
                <!-- WhatsApp in Footer -->
                <div class="mt-8 flex items-center gap-3">
                    <i class="fab fa-whatsapp text-3xl md:text-4xl text-green-500"></i>
                    <div>
                        <a href="https://wa.me/919177784328" target="_blank" rel="noopener noreferrer" class="text-lg md:text-2xl font-semibold hover:text-green-400 transition">+91 91777 84328</a>
                        <p class="text-xs text-green-400">Bookings accepted only on this number</p>
                    </div>
                </div>
            </div>
            
            <div class="md:col-span-2">
                <h4 class="font-semibold mb-6 text-base md:text-lg">Quick Links</h4>
                <ul class="space-y-3 text-gray-400 text-sm">
                    <li><a href="#collections" class="hover:text-white transition">All Collections</a></li>
                    <li><a href="#araba" class="hover:text-white transition">Araba Slippers</a></li>
                    <li><a href="#dailywear" class="hover:text-white transition">Daily Wear</a></li>
                    <li><a href="#underwear" class="hover:text-white transition">Underwear</a></li>
                    <li><a href="#banyans" class="hover:text-white transition">Banyans</a></li>
                </ul>
            </div>
            
            <div class="md:col-span-5">
                <h4 class="font-semibold mb-6 text-base md:text-lg">Visit Our Store</h4>
                <p class="text-gray-400 text-sm md:text-base">MS Shoe Hub<br>Falaknuma, Hyderabad, Telangana 500053</p>
                <p class="text-xs text-gray-500 mt-8">© 2025 MS Shoe Hub. All Rights Reserved.<br>Made with ❤️ for quality & service</p>
            </div>
        </div>
    </footer>

    <script>
        // ==================== PRODUCT DATA ====================
        const products = {
            araba: [
                { img: "https://ibb.co/vCRXxmMk", name: "Classic Tan Araba Slipper", price: "449", original: "599" },
                { img: "https://ibb.co/ZpQM1Hsq", name: "Royal Black Araba", price: "499", original: "649" },
                { img: "https://ibb.co/pvf0nKbr", name: "Dual-Tone Brown Araba", price: "549", original: "699" },
                { img: "https://ibb.co/4wQbjFvP", name: "Premium Cream Araba", price: "599", original: "749" },
                { img: "https://ibb.co/XZj1JNjg", name: "Modern Grey Araba", price: "429", original: "579" },
                { img: "https://ibb.co/5NHHm8V", name: "Navy Blue Araba Slipper", price: "479", original: "629" },
                { img: "https://ibb.co/spFyjf35", name: "Rustic Brown Ethnic Araba", price: "399", original: "549" },
                { img: "https://ibb.co/Jjmz9CQ3", name: "Olive Green Araba", price: "519", original: "669" },
                { img: "https://ibb.co/JWSLVFRX", name: "Coffee Brown Premium Araba", price: "559", original: "719" },
                { img: "https://ibb.co/JWkrX99J", name: "Matte Black Araba", price: "469", original: "619" },
                { img: "https://ibb.co/xrW2PG5", name: "Golden Tan Araba", price: "539", original: "689" },
                { img: "https://ibb.co/FbQqW4LP", name: "Deep Burgundy Araba", price: "499", original: "649" },
                { img: "https://ibb.co/Y4YFDfGP", name: "Slate Grey Comfort Araba", price: "409", original: "559" },
                { img: "https://ibb.co/YTKFdZpz", name: "Light Beige Araba", price: "579", original: "729" },
                { img: "https://ibb.co/0jff0QBh", name: "Charcoal Black Araba", price: "459", original: "609" },
                { img: "https://ibb.co/4RcY4VzD", name: "Warm Brown Dual Strap Araba", price: "529", original: "679" },
                { img: "https://ibb.co/WvtfSpWK", name: "Sandstone Beige Araba", price: "389", original: "529" },
                { img: "https://ibb.co/dx8ZQF8", name: "Forest Green Araba", price: "509", original: "659" },
                { img: "https://ibb.co/HTtMSPCS", name: "Rich Mahogany Araba", price: "569", original: "719" },
                { img: "https://ibb.co/spGfnpKz", name: "Soft Grey Ethnic Araba", price: "439", original: "589" },
                { img: "https://ibb.co/hxYfQG37", name: "Cognac Brown Araba", price: "549", original: "699" },
                { img: "https://ibb.co/8nrLbG7p", name: "Midnight Blue Araba", price: "419", original: "569" },
                { img: "https://ibb.co/zVVcDbsc", name: "Rustic Tan Premium Araba", price: "589", original: "739" },
                { img: "https://ibb.co/JWnnbG6h", name: "Dark Olive Araba", price: "479", original: "629" },
                { img: "https://ibb.co/Ps0HXWrC", name: "Classic Black Strap Araba", price: "499", original: "649" },
                { img: "https://ibb.co/Y4Rxwz9F", name: "Warm Terracotta Araba", price: "529", original: "679" },
                { img: "https://ibb.co/S48wrnCY", name: "Light Grey Modern Araba", price: "409", original: "559" },
                { img: "https://ibb.co/vvwVZdtL", name: "Deep Brown Ethnic Araba", price: "559", original: "709" },
                { img: "https://ibb.co/mVfd2Gxt", name: "Signature Tan Araba", price: "599", original: "749" }
            ],
            daily: [
                { img: "https://ibb.co/xSn5vzG4", name: "Classic Black Daily Slipper", price: "499", original: "" },
                { img: "https://ibb.co/8nVGp7HC", name: "Navy Blue Comfort Slipper", price: "499", original: "" },
                { img: "https://ibb.co/xKgZWvWR", name: "Brown Everyday Slipper", price: "499", original: "" },
                { img: "https://ibb.co/Kc37Z5YF", name: "Grey Rubber Flip Flop", price: "499", original: "" },
                { img: "https://ibb.co/bMv5cJWJ", name: "Black Mesh Daily Wear", price: "499", original: "" },
                { img: "https://ibb.co/5xFdcxBR", name: "Tan Casual Slipper", price: "499", original: "" },
                { img: "https://ibb.co/BXtYp6z", name: "Olive Green Daily Slipper", price: "499", original: "" },
                { img: "https://ibb.co/tww3sm8s", name: "Red Accent Comfort Slipper", price: "499", original: "" },
                { img: "https://ibb.co/p6s3mQVw", name: "Navy Sporty Daily Wear", price: "499", original: "" },
                { img: "https://ibb.co/xSkhGdzw", name: "Charcoal Grey Flip Flop", price: "499", original: "" },
                { img: "https://ibb.co/hFcqBNgq", name: "Brown Textured Slipper", price: "499", original: "" },
                { img: "https://ibb.co/Q72nPpYj", name: "Black Premium Daily Slipper", price: "499", original: "" },
                { img: "https://ibb.co/BK6wtR9X", name: "Blue Casual Comfort Slipper", price: "499", original: "" },
                { img: "https://ibb.co/zhkgrsdT", name: "White & Grey Daily Wear", price: "499", original: "" },
                { img: "https://ibb.co/jZh2P8TT", name: "Tan Rubber Slipper", price: "499", original: "" },
                { img: "https://ibb.co/xqcy9qTY", name: "Dark Brown Everyday Slipper", price: "499", original: "" },
                { img: "https://ibb.co/MxKDgt2n", name: "Black Sport Daily Slipper", price: "499", original: "" },
                { img: "https://ibb.co/Z1LQmMGz", name: "Olive Mesh Comfort Slipper", price: "499", original: "" },
                { img: "https://ibb.co/wZ1wCD9Z", name: "Grey Textured Daily Wear", price: "499", original: "" },
                { img: "https://ibb.co/0yBQgBmx", name: "Navy Blue Flip Flop", price: "499", original: "" },
                { img: "https://ibb.co/kszPYjRF", name: "Brown Classic Slipper", price: "499", original: "" },
                { img: "https://ibb.co/bqnt7F8", name: "Black Bold Daily Slipper", price: "499", original: "" },
                { img: "https://ibb.co/m5vHTrrF", name: "Red & Black Sport Slipper", price: "499", original: "" },
                { img: "https://ibb.co/TqxfV6Vr", name: "Tan Modern Daily Wear", price: "499", original: "" },
                { img: "https://ibb.co/XrGCvmh2", name: "Grey Premium Slipper", price: "499", original: "" },
                { img: "https://ibb.co/7xXtTWbT", name: "Navy Comfort Flip Flop", price: "499", original: "" },
                { img: "https://ibb.co/XkpvGGmr", name: "Olive Green Daily Slipper", price: "499", original: "" },
                { img: "https://ibb.co/gFS3gL99", name: "Black Mesh Daily Wear", price: "499", original: "" },
                { img: "https://ibb.co/nsmvLytz", name: "Brown Textured Slipper", price: "499", original: "" },
                { img: "https://ibb.co/Y7MXcWVg", name: "Charcoal Grey Daily Slipper", price: "499", original: "" },
                { img: "https://ibb.co/1GDtrgGT", name: "Tan Sporty Daily Wear", price: "499", original: "" },
                { img: "https://ibb.co/F4DS3MKW", name: "Navy Blue Everyday Slipper", price: "499", original: "" },
                { img: "https://ibb.co/nsZgmF8q", name: "Black Classic Daily Slipper", price: "499", original: "" }
            ],
            underwear: [
                { img: "https://ibb.co/4RGJqBcz", name: "Dixcy Scott Macho Trunk (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/FbchP2yR", name: "Dixcy Scott Cotton Brief (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/qKQJmBc", name: "Dixcy Scott Premium Trunk (5 Pack)", price: "399", original: "549", pack: "5" },
                { img: "https://ibb.co/r2jpyQKv", name: "Dixcy Scott Boxer Brief (Single)", price: "129", original: "169", pack: "" },
                { img: "https://ibb.co/d02JMXmQ", name: "Dixcy Scott Comfort Trunk (3 Pack)", price: "299", original: "399", pack: "3" },
                { img: "https://ibb.co/twXBXjmX", name: "Dixcy Scott Ribbed Brief (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/3mJtVXwR", name: "Dixcy Scott Classic Trunk (5 Pack)", price: "399", original: "549", pack: "5" },
                { img: "https://ibb.co/sdXQdMvR", name: "Dixcy Scott Macho Brief (Single)", price: "99", original: "149", pack: "" }
            ],
            banyans: [
                { img: "https://ibb.co/GQD97BQd", name: "Dixcy Scott Cotton Vest (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/bjCJL146", name: "Dixcy Scott Ribbed Banian (3 Pack)", price: "299", original: "399", pack: "3" },
                { img: "https://ibb.co/XZvRVYfz", name: "Dixcy Scott Premium Vest (5 Pack)", price: "399", original: "549", pack: "5" },
                { img: "https://ibb.co/mC1mpmtM", name: "Rupa Thermocot Vest (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/wZkWYr3y", name: "Rupa Jon Sleeveless Banian (Single)", price: "99", original: "149", pack: "" },
                { img: "https://ibb.co/RGBg5Kkw", name: "Rupa Classic Vest (5 Pack)", price: "399", original: "549", pack: "5" },
                { img: "https://ibb.co/BK2sqKLB", name: "Rupa Softline Vest (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/p6JVj5tJ", name: "Rupa Premium Banian (Single)", price: "129", original: "169", pack: "" },
                { img: "https://ibb.co/5xT11J1t", name: "Rupa Cotton Vest (3 Pack)", price: "299", original: "399", pack: "3" },
                { img: "https://ibb.co/WpM67BG3", name: "Rupa Ribbed Banian (5 Pack)", price: "399", original: "549", pack: "5" },
                { img: "https://ibb.co/k2x9XJzQ", name: "Rupa Premium Vest (Single)", price: "99", original: "149", pack: "" },
                { img: "https://ibb.co/XftMSXn2", name: "Rupa Classic Banian (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/cXbDd7Qy", name: "Essa Cotton Banian (Single)", price: "99", original: "149", pack: "" },
                { img: "https://ibb.co/jZMFQY57", name: "Essa Premium Vest (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/W46RpFG2", name: "Essa Ribbed Cotton Vest (5 Pack)", price: "399", original: "549", pack: "5" },
                { img: "https://ibb.co/sdzJsLg9", name: "Essa Classic Banian (3 Pack)", price: "299", original: "399", pack: "3" },
                { img: "https://ibb.co/2DZb4Ym", name: "Essa Sleeveless Vest (Single)", price: "109", original: "159", pack: "" },
                { img: "https://ibb.co/XfP2dcL2", name: "Essa Premium Banian (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/BVx3TvyF", name: "Essa Cotton Vest (5 Pack)", price: "399", original: "549", pack: "5" },
                { img: "https://ibb.co/hFPLyYhG", name: "Essa Ribbed Vest (Single)", price: "99", original: "149", pack: "" },
                { img: "https://ibb.co/mV6pKYJY", name: "Essa Classic Vest (3 Pack)", price: "299", original: "399", pack: "3" },
                { img: "https://ibb.co/ZzYRnNkJ", name: "Essa Premium Sleeveless Banian (3 Pack)", price: "249", original: "349", pack: "3" },
                { img: "https://ibb.co/k2GcffS9", name: "Essa Soft Cotton Vest (5 Pack)", price: "399", original: "549", pack: "5" }
            ]
        };

        // Render function
        function renderProducts(containerId, items) {
            const container = document.getElementById(containerId);
            if (!container) {
                console.error(`Container with ID "${containerId}" not found`);
                return;
            }
            
            container.innerHTML = '';
            
            items.forEach(item => {
                const discount = item.original ? Math.round(((parseInt(item.original) - parseInt(item.price)) / parseInt(item.original)) * 100) : 0;

                const cardHTML = `
                <div class="product-card bg-white rounded-3xl overflow-hidden border border-gray-100">
                    <div class="relative bg-gray-200">
                        <img src="${item.img}" alt="${item.name}" class="w-full h-64 object-cover" onerror="this.src='https://via.placeholder.com/250x250?text=Image+Not+Found'">
                        ${discount > 0 ? `<div class="absolute top-4 left-4 bg-red-600 text-white text-xs font-bold px-3 py-1 rounded-full">${discount}% OFF</div>` : ''}
                    </div>
                    <div class="p-5">
                        <h3 class="font-semibold text-sm md:text-base line-clamp-2 mb-1">${item.name}</h3>
                        ${item.pack ? `<p class="text-xs text-gray-500 mb-2">Pack: ${item.pack}</p>` : ''}
                        <div class="flex items-baseline gap-2">
                            <span class="text-xl md:text-2xl font-bold">₹${item.price}</span>
                            ${item.original ? `<span class="text-gray-400 line-through text-xs md:text-sm">₹${item.original}</span>` : ''}
                        </div>
                    </div>
                </div>`;
                container.innerHTML += cardHTML;
            });
        }

        // Render all sections on load
        window.addEventListener('load', function() {
            try {
                renderProducts('araba-grid', products.araba);
                renderProducts('daily-grid', products.daily);
                renderProducts('underwear-grid', products.underwear);
                renderProducts('banyans-grid', products.banyans);
                
                console.log('%c✅ MS Shoe Hub - All products loaded successfully!', 'color:#000;font-size:16px;font-weight:bold');
                console.log('Araba: 29 | Daily Wear: 32 | Underwear: 8 | Banyans: 23');
            } catch (error) {
                console.error('Error loading products:', error);
            }
        });

        // Smooth scroll behavior
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });
    </script>
</body>
</html>
