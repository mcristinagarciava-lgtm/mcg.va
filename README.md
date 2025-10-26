<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Maria Cristina Garcia - Executive Virtual Assistant</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
    
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest/dist/umd/lucide.min.js"></script>

    <!-- Swiper JS for Testimonials -->
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css" />
    <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

    <style>
        :root {
            --azure-dark: #3f9dd1;
            --azure-light: #66aedd;
            --pastel-pink: #f27ea9;
            --orange-primary: #faaf20;
            --orange-light: #ffdf99;
            
            --bg-light: #f8f9fa; /* A very light gray for alternating sections */
            --text-dark: #1f2937; /* Dark gray for text */
            --text-light: #6b7280; /* Lighter gray for paragraphs */
        }

        html, body {
            overflow-x: hidden; /* Prevents horizontal scrollbar */
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: #ffffff;
        }

        /* Custom Tailwind Colors */
        .bg-azure-dark { background-color: var(--azure-dark); }
        .text-azure-dark { color: var(--azure-dark); }
        .border-azure-dark { border-color: var(--azure-dark); }

        .bg-azure-light { background-color: var(--azure-light); }
        .text-azure-light { color: var(--azure-light); }

        .bg-pastel-pink { background-color: var(--pastel-pink); }
        .text-pastel-pink { color: var(--pastel-pink); }
        .border-pastel-pink { border-color: var(--pastel-pink); }

        .bg-orange-primary { background-color: var(--orange-primary); }
        .text-orange-primary { color: var(--orange-primary); }
        .border-orange-primary { border-color: var(--orange-primary); }
        .hover\:bg-orange-primary-dark:hover { background-color: #e19e1c; }
        
        .bg-orange-light { background-color: var(--orange-light); }
        .text-orange-light { color: var(--orange-light); }
        
        .bg-bg-light { background-color: var(--bg-light); }
        .text-text-dark { color: var(--text-dark); }
        .text-text-light { color: var(--text-light); }
        .bg-text-dark { background-color: var(--text-dark); }

        /* Hero Background Gradient */
        .hero-bg {
            background: linear-gradient(135deg, var(--azure-light), var(--pastel-pink));
            opacity: 0.1;
            filter: blur(100px);
        }

        /* Flip Card Base Style */
        .flip-card {
            perspective: 1000px;
        }
        .flip-card-inner {
            position: relative;
            width: 100%;
            height: 100%;
            transition: transform 0.6s;
            transform-style: preserve-3d;
        }
        .flip-card:hover .flip-card-inner {
            transform: rotateY(180deg);
        }
        .flip-card-front, .flip-card-back {
            position: absolute;
            width: 100%;
            height: 100%;
            -webkit-backface-visibility: hidden;
            backface-visibility: hidden;
            border-radius: 1rem; /* 16px */
        }
        .flip-card-back {
            transform: rotateY(180deg);
            overflow-y: auto; /* Add scroll for overflowing text */
            -ms-overflow-style: none;  /* IE and Edge */
            scrollbar-width: none;  /* Firefox */
        }
        /* Hide scrollbar for Chrome, Safari and Opera */
        .flip-card-back::-webkit-scrollbar {
            display: none;
        }


        /* Testimonial Slider */
        .swiper-pagination-bullet-active {
            background-color: var(--azure-dark) !important;
        }
        .swiper-button-next, .swiper-button-prev {
            color: var(--azure-dark) !important;
        }

        /* Scroll Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .fade-in-up {
            animation: fadeInUp 0.8s ease-out forwards;
            opacity: 0;
        }
    </style>
</head>
<body class="text-text-dark">

    <main>
        
        <!-- ========== HERO (UPDATED) ========== -->
        <section id="home" class="pt-20 pb-12 md:pt-24 md:pb-16 flex items-center bg-bg-light relative overflow-hidden">
            <div class="hero-bg absolute inset-0"></div>
            <div class="container mx-auto px-6 text-center relative z-10">
                
                <h1 id="typing-text" class="text-4xl md:text-6xl font-extrabold text-text-dark mb-4 h-20 md:h-16"></h1>
                
                <!-- EDITED: Shortened text and changed color -->
                <p class="text-lg md:text-xl text-azure-light font-medium leading-tight mb-2">
                    Executive VA | Customer Support
                </p>
                <p class="text-lg md:text-xl text-azure-light font-medium leading-tight mb-6">
                    E-commerce VA | Admin Support
                </p>
                
                <p class="text-xl md:text-2xl text-text-dark max-w-2xl mx-auto mb-8">
                    Your business's new best friend. I handle the chaos so you can focus on the magic.
                </p>
                
                <!-- EDITED: Changed button text -->
                <a href="https://calendly.com/mcristinagarcia-va/30min" target="_blank" rel="noopener noreferrer" class="inline-block bg-azure-dark text-white font-bold py-3 px-8 rounded-full text-lg shadow-lg hover:bg-azure-dark/90 transition duration-300 transform hover:scale-105">
                    Schedule a Meeting
                </a>
            </div>
        </section>

        <!-- ========== ABOUT ME ========== -->
        <section id="about" class="py-12 md:py-16">
            <div class="container mx-auto px-6 max-w-4xl text-center fade-in-up">
                <span class="text-orange-primary font-bold tracking-wider uppercase">About Me</span>
                <h2 class="text-3xl md:text-4xl font-bold text-text-dark mt-2 mb-6 flex items-center justify-center">
                    Hi, I’m MARIA! 
                    <i data-lucide="smile" class="w-8 h-8 text-orange-primary ml-2"></i>
                </h2>
                <p class="text-lg text-text-light leading-relaxed mb-4">
                    Your go-to Virtual Assistant for all things admin, social, and seriously organized.
                </p>
                <p class="text-lg text-text-light leading-relaxed mb-4">
                    I help busy professionals, business owners, and teams keep things running smoothly behind the scenes — from managing emails and calendars to creating social media content and keeping records in check.
                </p>
                <p class="text-lg text-text-light leading-relaxed">
                    With a background supporting healthcare providers, small business owners, and executives, I know how to juggle moving parts while staying calm, reliable, and on top of the details. I’m quick to learn, easy to work with, and always ready to jump in where you need me most. Let’s make your day a little lighter!
                </p>
            </div>
        </section>

        <!-- ========== SERVICES (Flip Cards) ========== -->
        <section id="services" class="py-12 md:py-16 bg-bg-light">
            <div class="container mx-auto px-6">
                <div class="text-center max-w-3xl mx-auto fade-in-up">
                    <span class="text-orange-primary font-bold tracking-wider uppercase">Services</span>
                    <h2 class="text-3xl md:text-4xl font-bold text-text-dark mt-2 mb-4">What I Do Best</h2>
                    <p class="text-lg text-text-light mb-12">
                        I offer a range of services to free up your time. Hover over a card to see the details!
                    </p>
                </div>

                <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8 fade-in-up">
                    
                    <!-- Card 1: Ecommerce -->
                    <div class="flip-card h-[450px]">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-dark">
                                <div class="w-20 h-20 bg-azure-light/20 text-azure-dark rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="shopping-cart" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Ecommerce Specialist</h3>
                            </div>
                            <div class="flip-card-back bg-azure-dark text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Ecommerce Specialist</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Product Research</li>
                                    <li>Listing Management & Store Management</li>
                                    <li>Graphic Design</li>
                                    <li>Creating Cases For Reimbursements</li>
                                    <li>Customer Service</li>
                                    <li>Respond to Reviews and Feedback</li>
                                    <li>Creating Shipment Plan</li>
                                    <li>Keyword Tracking & Research</li>
                                    <li>Creating SOPs</li>
                                    <li>Reporting & Optimizations</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Card 2: Social Media -->
                    <div class="flip-card h-[450px]">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-pastel-pink">
                                <div class="w-20 h-20 bg-pastel-pink/20 text-pastel-pink rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="share-2" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Social Media Manager</h3>
                            </div>
                            <div class="flip-card-back bg-pastel-pink text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Social Media Manager</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Content Creation & Custom Graphics</li>
                                    <li>Content Planning & Calendars</li>
                                    <li>Post Scheduling (FB, IG, LinkedIn)</li>
                                    <li>Consistent, Optimized Posting</li>
                                    <li>Community Management (Comments & DMs)</li>
                                    <li>Audience Engagement</li>
                                    <li>Performance Reports & Analytics</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Card 3: Admin VA -->
                    <div class="flip-card h-[450px]">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-orange-primary">
                                <div class="w-20 h-20 bg-orange-light/30 text-orange-primary rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="clipboard-user" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Executive / Admin VA</h3>
                            </div>
                            <div class="flip-card-back bg-orange-primary text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Executive / Admin VA</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Email & Calendar Management</li>
                                    <li>Research & Reporting</li>
                                    <li>Recruitment Support</li>
                                    <li>Social Media Account Setup & Mgt.</li>
                                    <li>Blog Management (Basic WordPress)</li>
                                    <li>Client Inquiries (Phone/Email)</li>
                                    <li>Light Bookkeeping</li>
                                    <li>Graphic Design (Flyers)</li>
                                    <li>Video & Photo Editing</li>
                                    <li>Data Entry</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Card 4: Other Skills -->
                    <div class="flip-card h-[450px]">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-light">
                                <div class="w-20 h-20 bg-azure-light/20 text-azure-light rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="sparkles" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Other Skills</h3>
                            </div>
                            <div class="flip-card-back bg-azure-light text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Other Skills</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Website Creation (Wix, WordPress)</li>
                                    <li>Order Fulfillment</li>
                                    <li>Inventory Management</li>
                                    <li>Return Management</li>
                                    <li>Facebook and Google Ads</li>
                                    <li>Hubspot Ticket Management</li>
                                    <li>AI Prompting (ChatGPT & Gemini)</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- ========== TECH TOOLKIT (Flip Cards) ========== -->
        <section id="tools" class="py-12 md:py-16">
            <div class="container mx-auto px-6 fade-in-up">
                <div class="text-center max-w-3xl mx-auto">
                    <span class="text-orange-primary font-bold tracking-wider uppercase">My Tech Toolkit</span>
                    <h2 class="text-3xl md:text-4xl font-bold text-text-dark mt-2 mb-12 flex items-center justify-center">
                        <i data-lucide="briefcase" class="w-8 h-8 text-orange-primary mr-3"></i>
                        Programs, Tools, & Apps I Use
                    </h2>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    
                    <!-- Tool Card 1: Admin -->
                    <div class="flip-card h-80">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-dark">
                                <div class="w-20 h-20 bg-azure-light/20 text-azure-dark rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="folders" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Admin & PM</h3>
                            </div>
                            <div class="flip-card-back bg-azure-dark text-white p-6">
                                <h3 class="text-xl font-bold mb-3">🗂️ Admin & PM</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Google Workspace</li>
                                    <li>Microsoft Excel</li>
                                    <li>Dropbox</li>
                                    <li>Monday.com | ClickUp</li>
                                    <li>Asana | Trello</li>
                                    <li>TeamViewer | AnyDesk</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Tool Card 2: CRM -->
                    <div class="flip-card h-80">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-pastel-pink">
                                <div class="w-20 h-20 bg-pastel-pink/20 text-pastel-pink rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="message-circle" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Communication & CRM</h3>
                            </div>
                            <div class="flip-card-back bg-pastel-pink text-white p-6">
                                <h3 class="text-xl font-bold mb-3">💬 Communication & CRM</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>HubSpot / Freshdesk / Gorgias</li>
                                    <li>Slack</li>
                                    <li>Dialpad</li>
                                    <li>Pipedrive</li>
                                    <li>ActiveCampaign</li>
                                    <li>Jane | Halaxy</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Tool Card 3: E-Commerce -->
                    <div class="flip-card h-80">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-orange-primary">
                                <div class="w-20 h-20 bg-orange-light/30 text-orange-primary rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="store" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">E-Commerce & Sales</h3>
                            </div>
                            <div class="flip-card-back bg-orange-primary text-white p-6">
                                <h3 class="text-xl font-bold mb-3">🛒 E-Commerce & Sales</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Amazon Seller Central</li>
                                    <li>Shopify</li>
                                    <li>Ideal Dealer Portal</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Tool Card 4: Design -->
                    <div class="flip-card h-80">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-light">
                                <div class="w-20 h-20 bg-azure-light/20 text-azure-light rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="palette" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Design & Content</h3>
                            </div>
                            <div class="flip-card-back bg-azure-light text-white p-6">
                                <h3 class="text-xl font-bold mb-3">🎨 Design & Content</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Canva</li>
                                    <li>Adobe Photoshop</li>
                                    <li>Filmora</li>
                                    <li>Davinci Resolve</li>
                                    <li>CapCut</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Tool Card 5: Marketing -->
                    <div class="flip-card h-80">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-dark">
                                <div class="w-20 h-20 bg-azure-light/20 text-azure-dark rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="bar-chart-3" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Marketing & Tracking</h3>
                            </div>
                            <div class="flip-card-back bg-azure-dark text-white p-6">
                                <h3 class="text-xl font-bold mb-3">📈 Marketing & Tracking</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Google Ads</li>
                                    <li>Google Tag Manager</li>
                                    <li>Meta Business Suite</li>
                                    <li>Google Analytics</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Tool Card 6: CMS -->
                    <div class="flip-card h-80">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-pastel-pink">
                                <div class="w-20 h-20 bg-pastel-pink/20 text-pastel-pink rounded-full flex items-center justify-center mb-4">
                                    <i data-lucide="globe-2" class="w-10 h-10"></i>
                                </div>
                                <h3 class="text-2xl font-bold text-text-dark">Website & CMS</h3>
                            </div>
                            <div class="flip-card-back bg-pastel-pink text-white p-6">
                                <h3 class="text-xl font-bold mb-3">🌐 Website & CMS</h3>
                                <ul class="space-y-2 text-sm list-disc list-inside text-left">
                                    <li>Wix</li>
                                    <li>WordPress</li>
                                    <li>Square</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>


        <!-- ========== PORTFOLIO ========== -->
        <section id="portfolio" class="py-12 md:py-16 bg-bg-light">
            <div class="container mx-auto px-6 fade-in-up">
                <div class="text-center max-w-3xl mx-auto">
                    <span class="text-orange-primary font-bold tracking-wider uppercase">Portfolio</span>
                    <h2 class="text-3xl md:text-4xl font-bold text-text-dark mt-2 mb-12">See My Skills in Action</h2>
                </div>
                
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <div class="bg-white p-6 rounded-lg shadow-lg text-center transition-transform transform hover:scale-105">
                        <i data-lucide="palette" class="w-12 h-12 text-pastel-pink mx-auto mb-4"></i>
                        <h3 class="text-xl font-semibold mb-2">Graphic Design</h3>
                        <p class="text-text-light">Branding materials, social media graphics, and flyers created with Canva & Photoshop.</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-lg text-center transition-transform transform hover:scale-105">
                        <i data-lucide="store" class="w-12 h-12 text-azure-dark mx-auto mb-4"></i>
                        <h3 class="text-xl font-semibold mb-2">E-commerce Management</h3>
                        <p class="text-text-light">Optimized product listings for Amazon & Shopify, including SEO and inventory management.</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-lg text-center transition-transform transform hover:scale-105">
                        <i data-lucide="video" class="w-12 h-12 text-orange-primary mx-auto mb-4"></i>
                        <h3 class="text-xl font-semibold mb-2">Content Creation</h3>
                        <p class="text-text-light">Engaging video shorts for TikTok & FB Reels, edited with Filmora & CapCut.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- ========== WORK EXPERIENCE (Flip Cards) ========== -->
        <section id="experience" class="py-12 md:py-16">
            <div class="container mx-auto px-6 max-w-7xl fade-in-up">
                <div class="text-center max-w-3xl mx-auto">
                    <span class="text-orange-primary font-bold tracking-wider uppercase">My Journey</span>
                    <h2 class="text-3xl md:text-4xl font-bold text-text-dark mt-2 mb-16">Work Experience</h2>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-8">
                    
                    <!-- Experience 1 -->
                    <div class="flip-card h-72">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-dark">
                                <span class="text-sm font-medium text-azure-dark mb-2">2024 - 2025</span>
                                <h3 class="text-2xl font-bold text-text-dark">Intake Specialist</h3>
                                <h4 class="text-lg font-semibold text-text-light mt-1">Precision Compounding</h4>
                            </div>
                            <div class="flip-card-back bg-azure-dark text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Intake Specialist</h3>
                                <p class="text-sm">Accurately entered and verified patient/prescription data, ensuring 100% HIPAA compliance and smooth pharmacy processing.</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Experience 2 -->
                    <div class="flip-card h-72">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-pastel-pink">
                                <span class="text-sm font-medium text-pastel-pink mb-2">2022 - 2025</span>
                                <h3 class="text-2xl font-bold text-text-dark">Admin Assistant</h3>
                                <h4 class="text-lg font-semibold text-text-light mt-1">District Performance</h4>
                            </div>
                            <div class="flip-card-back bg-pastel-pink text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Admin Assistant</h3>
                                <p class="text-sm">Managed appointments and cancellations, submitted insurance claims, updated SOPs, and ensured smooth payment processing.</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Experience 3 -->
                    <div class="flip-card h-72">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-orange-primary">
                                <span class="text-sm font-medium text-orange-primary mb-2">2022 - 2024</span>
                                <h3 class="text-2xl font-bold text-text-dark">Executive VA</h3>
                                <h4 class="text-lg font-semibold text-text-light mt-1">Goldenwest Lawnmower</h4>
                            </div>
                            <div class="flip-card-back bg-orange-primary text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Executive VA</h3>
                                <p class="text-sm">Managed orders, invoices, and financial reconciliations. Designed branding, packaging, brochures, and improved online listings.</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Experience 4 -->
                    <div class="flip-card h-72">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-light">
                                <span class="text-sm font-medium text-azure-light mb-2">2022 - 2024</span>
                                <h3 class="text-2xl font-bold text-text-dark">Virtual Assistant</h3>
                                <h4 class="text-lg font-semibold text-text-light mt-1">SolidGPS</h4>
                            </div>
                            <div class="flip-card-back bg-azure-light text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Virtual Assistant</h3>
                                <p class="text-sm">Designed logos, packaging, and product labels. Created marketing brochures, flyers, and produced TikTok/FB Reels content.</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Experience 5 -->
                    <div class="flip-card h-72">
                        <div class="flip-card-inner">
                            <div class="flip-card-front bg-white p-6 rounded-2xl shadow-lg flex flex-col justify-center items-center text-center border-t-4 border-azure-dark">
                                <span class="text-sm font-medium text-azure-dark mb-2">2021 - 2023</span>
                                <h3 class="text-2xl font-bold text-text-dark">Email Support</h3>
                                <h4 class="text-lg font-semibold text-text-light mt-1">Kickscrew LLC</h4>
                            </div>
                            <div class="flip-card-back bg-azure-dark text-white p-6">
                                <h3 class="text-xl font-bold mb-3">Email Support</h3>
                                <p class="text-sm">Resolved 100+ daily tickets (returns, refunds, shipping) and maintained high customer satisfaction during peak seasons.</p>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- ========== TESTIMONIALS ========== -->
        <section id="testimonials" class="py-12 md:py-16 bg-bg-light">
            <div class="container mx-auto px-6 max-w-4xl fade-in-up">
                <div class="text-center max-w-3xl mx-auto">
                    <span class="text-orange-primary font-bold tracking-wider uppercase">Testimonials</span>
                    <h2 class="text-3xl md:text-4xl font-bold text-text-dark mt-2 mb-12">What My Clients Say</h2>
                </div>

                <!-- Swiper -->
                <div class="swiper testimonial-slider relative">
                    <div class="swiper-wrapper">
                        <!-- Slide 1 -->
                        <div class="swiper-slide">
                            <div class="bg-white p-8 md:p-12 rounded-2xl shadow-lg max-w-2xl mx-auto text-center">
                                <i data-lucide="quote" class="w-16 h-16 text-pastel-pink/50 mx-auto"></i>
                                <p class="text-lg md:text-xl text-text-light italic leading-relaxed my-6">
                                    “Maria has become an integral member of our back office team. She helps us stay organized and on top of collections... It's incredibly valuable to have someone that we can turn to when small projects come up so that my time can be freed up to keep working on growing and managing the business.”
                                </p>
                                <h4 class="text-xl font-bold text-text-dark">Jesse L.</h4>
                                <span class="text-text-light">CEO</span>
                            </div>
                        </div>
                        <!-- Slide 2 -->
                        <div class="swiper-slide">
                            <div class="bg-white p-8 md:p-12 rounded-2xl shadow-lg max-w-2xl mx-auto text-center">
                                <i data-lucide="quote" class="w-16 h-16 text-pastel-pink/50 mx-auto"></i>
                                <p class="text-lg md:text-xl text-text-light italic leading-relaxed my-6">
                                    “Maria - once again very impressed. Probably best admin support I have seen in terms of setting expectations & explaining over the years. Know how I’m being charged, when, & distinctions on client vs. provider roles. Awesome! Also like how italics, bold, & font are used to highlight quick points at a glance.”
                                </p>
                                <h4 class="text-xl font-bold text-text-dark">Ward A.</h4>
                                <span class="text-text-light">CEO</span>
                            </div>
                        </div>
                    </div>
                    <!-- Add Pagination -->
                    <div class="swiper-pagination mt-8 relative"></div>
                    <!-- Add Navigation -->
                    <div class="swiper-button-next"></div>
                    <div class="swiper-button-prev"></div>
                </div>
            </div>
        </section>

        <!-- ========== CONTACT ========== -->
        <section id="contact" class="py-12 md:py-16 bg-azure-dark text-white">
            <div class="container mx-auto px-6 text-center z-10 relative fade-in-up">
                <div class="max-w-3xl mx-auto">
                    <h2 class="text-3xl md:text-4xl font-bold mt-6 mb-4">Ready to Lighten Your Workload?</h2>
                    <p class="text-lg leading-relaxed mb-8">
                        Let's chat! Book a free 30-minute consultation to discuss your needs and see how I can help you achieve your goals. No pressure, just a friendly conversation.
                    </p>
                    <a href="https://calendly.com/mcristinagarcia-va/30min" target="_blank" rel="noopener noreferrer" class="inline-block bg-pastel-pink text-white font-bold py-4 px-10 rounded-full text-lg shadow-lg hover:bg-pastel-pink/90 transition duration-300 transform hover:scale-105">
                        Schedule a Meeting
                    </a>
                </div>
            </div>
        </section>
    </main>

    <!-- ========== FOOTER ========== -->
    <footer class="bg-text-dark text-gray-400 py-8">
        <div class="container mx-auto px-6 text-center">
            <p>&copy; <span id="footer-year"></span> Maria Cristina Garcia. All rights reserved.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', (event) => {
            let iconsCreated = false;

            // 1. Create Icons (with retry)
            function createIcons() {
                if (typeof lucide !== 'undefined') {
                    lucide.createIcons();
                    iconsCreated = true;
                }
            }
            createIcons();
            // Retry if lucide was slow to load
            setTimeout(() => {
                if (!iconsCreated) createIcons();
            }, 500);

            
            // 2. Testimonial Slider
            if (typeof Swiper !== 'undefined') {
                new Swiper('.testimonial-slider', {
                    loop: true,
                    autoplay: {
                        delay: 5000,
                        disableOnInteraction: false,
                    },
                    pagination: {
                        el: '.swiper-pagination',
                        clickable: true,
                    },
                    navigation: {
                        nextEl: '.swiper-button-next',
                        prevEl: '.swiper-button-prev',
                    },
                    slidesPerView: 1,
                    spaceBetween: 30,
                });
            }

            // 3. Hero Typing Effect
            const typingTextElement = document.getElementById('typing-text');
            if (typingTextElement) {
                const textToType = "Maria Cristina Garcia";
                let charIndex = 0;
                
                function type() {
                    if (charIndex < textToType.length) {
                        typingTextElement.textContent += textToType.charAt(charIndex);
                        charIndex++;
                        setTimeout(type, 100);
                    }
                }
                type(); // Start typing
            }
            
            // 4. Scroll Animations
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        // Use a class to trigger the animation
                        entry.target.classList.add('is-visible');
                        observer.unobserve(entry.target);
                    }
                });
            }, {
                threshold: 0.1
            });
            
            document.querySelectorAll('.fade-in-up').forEach(el => {
                observer.observe(el);
            });
            
            // Add is-visible class to style block to define the animation
            const style = document.createElement('style');
            style.innerHTML = `
                .fade-in-up {
                    opacity: 0;
                    transform: translateY(30px);
                    transition: opacity 0.8s ease-out, transform 0.8s ease-out;
                }
                .fade-in-up.is-visible {
                    opacity: 1;
                    transform: translateY(0);
                }
            `;
            document.head.appendChild(style);


            // 5. Footer Year
            const footerYear = document.getElementById('footer-year');
            if (footerYear) {
                footerYear.textContent = new Date().getFullYear();
            }
        });
    </script>

</body>
</html>

